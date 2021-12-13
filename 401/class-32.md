# Permissions

> Authentication or identification by itself is not usually sufficient to gain access to information or code. For that, the entity requesting access must have authorization.

## How permissions are determined

- Before running the main body of the view each permission in the list is checked

- If any permission check fails, an exceptions.`PermissionDenied` or `exceptions.NotAuthenticated` exception will be raised

## Object level permissions

```python 

def get_object(self):
    obj = get_object_or_404(self.get_queryset(), pk=self.kwargs["pk"])
    self.check_object_permissions(self.request, obj)
    return obj

```

Limitations of object level permissions

For performance reasons the generic views will not automatically apply object level permissions to each instance in a queryset when returning a list of objects.


## Setting the permission policy

in setting.py we determine the default permission policy 

```python 
REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.IsAuthenticated',  #If not specified yse AllowAny
    ]
}
```

in views.py 

```python 

from rest_framework.permissions import IsAuthenticated
from rest_framework.response import Response
from rest_framework.views import APIView

class ExampleView(APIView):
    permission_classes = [IsAuthenticated]

    def get(self, request, format=None):
        content = {
            'status': 'request was permitted'
        }
        return Response(content)

# or you can use the  @api_view

from rest_framework.decorators import api_view, permission_classes
from rest_framework.permissions import IsAuthenticated
from rest_framework.response import Response

@api_view(['GET'])
@permission_classes([IsAuthenticated])
def example_view(request, format=None):
    content = {
        'status': 'request was permitted'
    }
    return Response(content)
```

resours

[DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)

