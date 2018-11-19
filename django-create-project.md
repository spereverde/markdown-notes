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





