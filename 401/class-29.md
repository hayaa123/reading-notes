# Custom User Model

Setup

To start, create a new Django project from the command line. We need to do several things:

create and navigate into a dedicated directory called accounts for our code
install Django

make a new Django project called config

make a new app accounts

start the local web server

Here are the commands to run:

```
$ cd ~/Desktop
$ mkdir accounts && cd accounts
$ pipenv install django~=3.1.0
$ pipenv shell
(accounts) $ django-admin.py startproject config .
(accounts) $ python manage.py startapp accounts
(accounts) $ python manage.py runserver
```

Custom User Model

- Creating our initial custom user model requires four steps:

- update config/settings.py
- create a new CustomUser model
- create new UserCreation and UserChangeForm
- update the admin

`touch accounts/forms.py`

```
touch accounts/forms.py
```


# Djano X

### Installation 

```
$ docker build .
$ docker-compose up -d
$ docker-compose exec web python manage.py migrate
$ docker-compose exec web python manage.py createsuperuser
# Load the site at http://127.0.0.1:8000
```

For Docker, the INTERNAL_IPS configuration in config/settings.py must be updated to the following:
```
# config/settings.py
# django-debug-toolbar
import socket
hostname, _, ips = socket.gethostbyname_ex(socket.gethostname())
INTERNAL_IPS = [ip[:-1] + "1" for ip in ips]
```


resorses 

[Django Best Practices: Custom User Model](https://learndjango.com/tutorials/django-custom-user-model)

[Django X](https://github.com/wsvincent/djangox)