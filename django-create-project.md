# django - creating a project

go to your usual projects folder

## activate virtualenv

`source ~/.virtualenvs/django/bin/activate`

## start a new django project

~~~
django-admin startproject kinsmanlibrary
cd kinsmanlibrary
~~~

## run the server

`python manage.py runserver`
- this will start the server, you can view the result at:
http://localhost:8000/

- **do not run the migration** it complains about when running the server the first time
- if you do run ´python manage.py migrate` it will create a db.sqlite3 file (= database)

- if you want to run your project on another port than the default :8000, you can use the following:

`python manage.py runserver 9000`

## stop the server

- Ctrl + C

## create a django application inside your django project

` python manage.py startapp books`

- this creates a books folderstructure containing all necessary files for a new django app

## running the migrations

- it complains about the migrations because it still needs to add the necessary migrations for the apps that were installed by Django
- you can find which apps it refers to by going to the settings.py file inside your djangoproject (not the django app), under INSTALLED_APPS
`python manage.py startapp books`

## add your new app to the installed apps

- go to the settings fiel of your django project (not the app) - INSTALLED_APPS
- add the name of your app to the list:

~~~
INSTALLED_APPS = [
    'books',
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
]
~~~

## add a model (table)

- in the models.py file of your app (not your project) add a new class and the necessarty fields for your new type of content, eg. a book
- model fields reference in Django:
https://docs.djangoproject.com/en/2.1/ref/models/fields/

## migrate and make migrations

`python manage.py makemigrations`

`python manage.py migrate`

`python manage.py dbshell`

https://code.visualstudio.com/docs/python/environments#_environment-variable-definitions-file
- this creates a books folderstructure containing all necessary files for a new django app
