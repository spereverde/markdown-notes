# django - creating a project

~~~
go to your usual projects folder
activate virtualenv:
source ~/.virtualenvs/django/bin/activate
django-admin startproject kinsmanlibrary
cd kinsmanlibrary
python manage.py runserver
python manage.py migrate (it complains first time running the server)
-> will create a db.sqlite3 file (= database)
stop the server
python manage.py startapp books
-> creates books folderstructure
~~~
