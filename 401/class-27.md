# Django Models

## Using Models

- help django to access and manage data

### Designing the LocalLibrary models

- When designing your models it makes sense to have separate models for every "object" 

- You might also want to use models to represent selection-list options

- Django allows you to define relationships that are one to one (OneToOneField), one to many (ForeignKey) and many to many (ManyToManyField).

### Model primer

**Model definition :**

- defined in an application's models.py file

```python 
from django.db import models

class MyModelName(models.Model):
    """A typical class defining a model, derived from the Model class."""

    # Fields --> A model can have an arbitrary number of fields, of any type
    my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')
    ...

    # Metadata
    class Meta:
        ordering = ['-my_field_name']

    # Methods -- >Minimally, in every model you should define the standard Python class method __str__() to return a human-readable string for each object.
    def get_absolute_url(self):
        """Returns the url to access a particular instance of MyModelName."""
        return reverse('model-detail-view', args=[str(self.id)])

    def __str__(self):
        """String for representing the MyModelName object (in Admin site etc.)."""
        return self.my_field_name
```

## Django admin site

- admin application can use your models to automatically build a site area that you can use to create

- The admin application can also be useful for managing data in production

- **Registering models** :

        ```python
        from django.contrib import admin
        from .models import Author, Genre, Book, BookInstance

        admin.site.register(Book)
        ```
- **Creating a superuser** : 

        `python3 manage.py createsuperuser`


