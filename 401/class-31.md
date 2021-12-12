# Django REST Framework & Docker

## Beginner’s Guide to Docker

- is a way to isolate and run entire applications. With Docker it doesn’t matter if you are using a Mac, Windows, or Linux computer anymore. The entire development environment is isolated

- Docker is a complex beast under the hood

- Docker is really just Linux containers

### Install Docker

- download the desktop app on our computer

- create account 

- if you are on Linux, you will need to add it manually. You can do this by running the command sudo pip install docker-compose after your Docker installation is complete.

## Django for APIs 

in views.py file 

```python 
from rest_framework import generics #####

from books.models import Book
from .serializers import BookSerializer


class BookAPIView(generics.ListAPIView): #####
    queryset = Book.objects.all()  #####
    serializer_class = BookSerializer
```

in serializers.py

`(library) $ touch api/serializers.py
`

```python 
from rest_framework import serializers #####

from books.models import Book


class BookSerializer(serializers.ModelSerializer): #####
    class Meta:
        model = Book
        fields = ('title', 'subtitle', 'author', 'isbn')
```

note we should add `'rest_framework',` in the setting installed apps (why ?) because it is a 3rd party app 

## resourses 

[Beginner’s Guide to Docker](https://wsvincent.com/beginners-guide-to-docker/)

[Django for APIs - Library Website](https://djangoforapis.com/library-website-and-api/)