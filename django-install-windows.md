# Django install notes - Windows 10


* [django docu](https://docs.djangoproject.com/en/2.0/howto/windows/)
* [github django project documentation](https://github.com/django/django/blob/master/docs/howto/windows.txt)

## install python

* as in the [django install python documentation](https://docs.djangoproject.com/en/2.0/howto/windows/#install-python)

## upgrade pip

* as you can read in the [install docu for pip](https://pip.pypa.io/en/latest/installing/), we don't need to install it, but it's better to make sure it's upgraded
 * *pip is already installed if you are using Python 2 >=2.7.9 or Python 3 >=3.4 downloaded from python.org or if you are working in a Virtual Environment created by virtualenv or pyvenv. Just make sure to upgrade pip.*

* open a command prompt in Windows:
 * type the windows key and type´cmd´ (it should show you a black icon with the name **Command Prompt**) and press enter or double click
* type `python -m pip install -U pip`

~~~
C:\Users\*username*
λ python -m pip install -U pip
Collecting pip
  Downloading pip-9.0.2-py2.py3-none-any.whl (1.4MB)
    100% |████████████████████████████████| 1.4MB 616kB/s
Installing collected packages: pip
  Found existing installation: pip 9.0.1
    Uninstalling pip-9.0.1:
      Successfully uninstalled pip-9.0.1
Successfully installed pip-9.0.2
~~~

## install and activate virtualenv

* as in the [django install virtualenv documentation](https://docs.djangoproject.com/en/2.0/howto/windows/#install-virtualenv-and-virtualenvwrapper)

~~~
C:\Users\*username*
λ pip install virtualenvwrapper-win
Collecting virtualenvwrapper-win
  Downloading virtualenvwrapper-win-1.2.5.tar.gz
Collecting virtualenv (from virtualenvwrapper-win)
  Downloading virtualenv-15.1.0-py2.py3-none-any.whl (1.8MB)
    100% |████████████████████████████████| 1.8MB 466kB/s
Installing collected packages: virtualenv, virtualenvwrapper-win
  Running setup.py install for virtualenvwrapper-win ... done
Successfully installed virtualenv-15.1.0 virtualenvwrapper-win-1.2.5
~~~

## install django

* as in the [django install django documentation](https://docs.djangoproject.com/en/2.0/howto/windows/#install-django)
~~~
C:\Users\*username*
(django) λ pip install django
Collecting django
  Downloading Django-2.0.3-py3-none-any.whl (7.1MB)
    100% |████████████████████████████████| 7.1MB 130kB/s
Collecting pytz (from django)
  Downloading pytz-2018.3-py2.py3-none-any.whl (509kB)
    100% |████████████████████████████████| 512kB 975kB/s
Installing collected packages: pytz, django
Successfully installed django-2.0.3 pytz-2018.3
~~~


# Windows using docker

* [docker compose docu](https://docs.docker.com/compose/django/)

