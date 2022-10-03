# Customized Django User

## Description:
* This is an example for using customized user configuration on Django.


## Environment:
Programing environment is as below.

* Python 3.10.7
* pip 22.2.2
* Django 4.1.1


## Application Installation Instructions:

    git clone https://github.com/kay1759/customized_django_user.git
    cd customized_django_user

* The original project name is 'webapp'
when you would like to change &lt;project name&gt;

    * change the directory name from 'webapp' to as you like
    * update settins.py for the value 'ROOT_URLCONF' and 'WSGI_APPLICATION' as your project name 

* Reset a branch to a specific tag & create tables


    git reset --hard &lt;tag name: example 'uuid'&gt;
    python manage.py makemigrations users
    python manage.py migrate


## Commit Tags:
### fullname:
* use full_name instead of first_name and last_name

### uuid:
* use UUID for Primary Key instead of auto increment integer


## Development
    * django-admin startproject webapp
    * cd webapp
    * python manage.py startapp users
    * create the classes AbstractUser, User in users/users.models
    * create the class UserAdmin in users/users.admin
    * add 'users' in 'INSTALLED_APPS' field in webapp.setting
    * add "AUTH_USER_MODEL = 'user.User'" in webapp.setting

## Licence:

[MIT]

## Author

[kay](https://github.com/kay1759)
