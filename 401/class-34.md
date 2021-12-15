# API Deployment

## Django Settings Best Practices

- Managing Django Settings: Issues

    - Different environments

    - Sensitive data

    - Sharing settings between team members

    - Django settings are a Python code

- Setting Configuration: Different Approaches

    There is no built-in universal way to configure Django settings without hardcoding them.

- Separate settings file for each environment

    ```
    settings/
    ├── __init__.py
    ├── base.py
    ├── ci.py
    ├── local.py
    ├── staging.py
    ├── production.py
    └── qa.py
    ```

    `python manage.py runserver --settings=settings.local`

## SSH 

 - Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet

 - The SSH command consists of 3 distinct parts:

        ssh {user}@{host}
 - There are three different encryption technologies used by SSH:

        1- Symmetrical encryption
        2-Asymmetrical encryption
        3-Hashing.  