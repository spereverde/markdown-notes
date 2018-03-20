# django - creating a project

~~~
go to your usual projects folder
activate virtualenv:
source ~/.virtualenvs/django/bin/activate
django-admin startproject kinsmanlibrary
cd kinsmanlibrary
python manage.py runserver
do not do the migration it complains about when running the server hte first time
if you do run
´python manage.py migrate`
it will create a db.sqlite3 file (= database)
stop the server
python manage.py startapp books
-> creates books folderstructure
~~~


