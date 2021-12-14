# Authentication & Production Server

## Introduction to JSON Web Tokens

- JSON Web Token (JWT) is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. 

- When should you use JSON Web Tokens?

  1- **Authorization**

  2- **Information Exchange**
  
- Information Exchange

  - JSON Web Tokens consist of three parts separated by dots (.), which are:

        Header -->The header typically consists of two parts: the type of the token, which is JWT, and the signing algorithm being used,  such as HMAC SHA256 or RSA.

        ```
        {
        "alg": "HS256",
        "typ": "JWT"
        }
        ```

        Payload --> which contains the claims. Claims are statements about an entity (typically, the user) and additional data. There are three types of claims: registered, public, and private claims.

        ```
        {
        "sub": "1234567890",
        "name": "John Doe",
        "admin": true
        }   
        ```

        Signature --> To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

    `xxxxx.yyyyy.zzzzz`

- How do JSON Web Tokens work?

    - when the user successfully logs in using their credentials, a JSON Web Token will be returned

    ![](https://cdn2.auth0.com/docs/media/articles/api-auth/client-credentials-grant.png)

- Why should we use JSON Web Tokens?

    - JSON is less verbose than XML, when it is encoded its size is also smaller, making JWT more compact than SAML (note :  This makes JWT a good choice to be passed in HTML and HTTP environments.)


    - JWT and SAML tokens can use a public/private key pair in the form of a X.509 certificate for signing. Signing XML with XML Digital Signature without introducing obscure security holes is very difficult when compared to the simplicity of signing JSON.

## How to Use JWT Authentication with Django REST Framework

- Installation & Setup

    1- `poetry add djangorestframework_simplejwt`

    2- in settings.py edit the authentication part

         REST_FRAMEWORK = {
         'DEFAULT_AUTHENTICATION_CLASSES': [
         'rest_framework_simplejwt.authentication .JWTAuthentication',
         ], 
        }

    3- in urls.py file we do the following 

        from django.urls import path
        from rest_framework_simplejwt import views as jwt_views

        urlpatterns = [
            # Your URLs...
            path('api/token/', jwt_views.TokenObtainPairView.as_view(), name='token_obtain_pair'),
            path('api/token/refresh/', jwt_views.TokenRefreshView.as_view(), name='token_refresh'),
        ]

    4- views.py in the app 

        from rest_framework.views import APIView
        from rest_framework.response import Response
        from rest_framework.permissions import IsAuthenticated


        class HelloView(APIView):
            permission_classes = (IsAuthenticated,)

            def get(self, request):
                content = {'message': 'Hello, World!'}
                return Response(content)

    5- urls.py in app 

        from django.urls import path
        from myapi.core import views

        urlpatterns = [
            path('hello/', views.HelloView.as_view(), name='hello'),
        ] 

## Django Runserver Is Not Your Production Server

If you want to run Django in production, be sure to use a production-ready web server like Nginx, and let your app be handled by a WSGI application server like Gunicorn.

If you plan on running on Heroku, a web server is provided implicitly. You don’t have to take care of it. You just need to specify a command to run your application server (again, Gunicorn is fine) in the Procfile.



[Introduction to JSON Web Tokens](https://jwt.io/introduction/)

[How to Use JWT Authentication with Django REST Framework](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)

[Django Runserver Is Not Your Production Server](https://vsupalov.com/django-runserver-in-production/)