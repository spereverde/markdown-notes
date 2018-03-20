# Django install notes

## macOS

* [django docu](https://docs.djangoproject.com/en/2.0/topics/install/)

* short verson:

~~~bash
download and install python3 from the python website
in your terminal:
$ mkdir ~/.virtualenvs
$ python3 -m venv ~/.virtualenvs/django 
$ source ~/.virtualenvs/django/bin/activate
$ cd ~/.virtualenvs/django
$ pip install Django
~~~

### 1. install python

* go to [https://www.python.org/downloads/](https://www.python.org/downloads/)
* Download the latest version for Mac OS X - *Download Python 3.6.4*
* Follow the steps from the install dialog

#### check to see that you have python3 installed

* open a Terminal (Launchpad, search for Terminal)
* type `python3 --version`
* this should show you `Python 3.6.4`
* typing `python --version` will show you the default python that is installed on your mac (Python 2.7.10), this is probably a python 2 version, just so you knwo that there are 2 versions of python living on your machine

#### do NOT install apache and mod_wsgi

### 2. install and activate a virtualenv

* when working with python, we usually need a virtualenv (virtual environment) to work in, basically so you don't screw something up on your real machine. You can find more info on the [virtualenv documentation](https://virtualenv.pypa.io/en/stable) 

#### create a space for your virtualenvs
* make a directory for your virtualenvs
* go to your Terminal
* I chose to create a folder called *.virtualenvs* in my homedir (~)
 * you can type a tilde (~) on a mac by typing *Option + n* 
 * your homedir on a mac is usually /Users/*your_user_name*
 * see [https://superuser.com/questions/158721/what-does-mean-in-terms-of-os-x-folders-directories](https://superuser.com/questions/158721/what-does-mean-in-terms-of-os-x-folders-directories) 
* type this command in the terminal: 
* `mkdir ~/.virtualenvs`

### 3.create a virtualenv specifically for your django project
* then use python 3 to create a virtualenv for django inside this folder:
* `python3 -m venv ~/.virtualenvs/django`
* more info on this in the [python venv docs](https://docs.python.org/3/library/venv.html)   

* note: we will probably use only one virtualenv, the django one, during the course. If you like you can also put the djangodev virtualenv in your homedir directly or somewhere else on your computer. If you will start other python projects, its usually handy to have a seperate virtualenv for each project, which is why I usually put them together in a virtualenvs folder so its clear to me where they are.

### 4.activate your django virtualenv

* `python3 -m venv ~/.virtualenvs/django`
* you will see that the virtualenv is activated when the name (in brackets) of the virtualenv is in front of your line in the terminal
* `(django) computername:~ username$`
* note: you will have to activate your django virtualenv everytime you restart your terminal (or computer)
*  you can manually deactivate the virtualenv by typing: `deactivate`

### 5.install django
* `cd ~/.virtualenvs/django`
* `pip install Django`

## Windows

* [django docu](https://docs.djangoproject.com/en/2.0/howto/windows/)
* [github django project documentation](https://github.com/django/django/blob/master/docs/howto/windows.txt)


## Windows using docker

* [docker compose docu](https://docs.docker.com/compose/django/)


