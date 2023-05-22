Do the «Writing your first Django app» instruction from Django documentation

1) Check if Django installed already

$ python3 -m django —version

My current Django version is 4.2.1

2) Creating a project
Auto-generates some code that establishes a Django project — a collection for an instance of Django:
  - database configuration
  - Django-specific options
  - application-specific settings

$ django-admin startproject mysite

unfortunately I didn’t have django-admin so I needed to install pip and django-admin

2a) 
$ curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py

2b) 
$ sudo ln -s /Users/svetlanamironova/Documents/repo/django-apps/simple-app/get-pip.py /usr/local/bin/get-pip.py

2c) 
$ cd /usr/local/bin/

2d)
$ sudo -H python3 get-pip.py

I can use environment variables for django:
(to isolate Python/Django settings of my project)

python3 -m venv myenv
source myenv/bin/activate
python3 -m pip install —upgrade pip
pip install django

the command 
$ django-admin startproject mysite 
now works

3) run app
$ cd mysite
$ python3 manage.py runserver

4) web server now works
go to http://127.0.0.1:8000
see «The install worked successfully! Congratulations!
You are seeing this page because DEBUG=True is in your settings file and you have not configured any URLs.»

5) input CTRL C to stop web server
