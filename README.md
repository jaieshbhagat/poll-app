# Polling Web Application Using Django
A web application submitted in fulfilment of the mini project in the subject of Open Source Technology Lab of fourth semester. The application had an admin login section whose roles included posting questions and corresponding options for the same.
The admin also can view the total number of votes done. Vote count of each of the options.
Front end used in built template engine of the framework and W3.CSS.

## Introduction
The Aim of this project is to create a fully functional poll website. A website, where end users are able to record their selected options and witness the at present results.

The website is managed by an Administrator account, through which website’s proprietor can add, delete, as well as modify the polls. The Administrator account also gives the possessor the authority to add and delete users.

The implementation revolves totally around Django, an open source web development framework, written in python.

## Methodology
The Django framework is based upon modelview-template architectural pattern. The models defines the database, the views maps to control and the template contains the appearance of the website. Besides Django, a python IDE named PyCham is used for easing the implementation process.

Using the Django framework’s pre-fabricated Administrative functionalities, an app called polls is created. All the models(databases) for the various webpages are implemented in a .sqlite3 database management system using the same framework. The templates for each webpage is created and the respective URLs are linked to these templates.

## Directory Structure
```
poll-app
│   db.sqlite3
│   manage.py
│   README.md
│
├───mysite
│   ├───settings.py
│   ├───urls.py
│   ├───wsgi.py
│   └───__init__.py
│
└───polls
    ├───admin.py
    ├───apps.py
    ├───models.py
    ├───tests.py
    ├───urls.py
    ├───views.py
    ├───__init__.py
    │
    ├───static
    │   └───polls
    │       ├───style.css
    │       │
    │       └───images
    │           ├───avatar2.png
    │           ├───avatar4.png
    │           └───background.jpg
    │
    └───templates
        ├───admin
        │   └───base_site.html
        │
        ├───polls
        │   ├───base.html
        │   ├───detail.html
        │   ├───index.html
        │   └───results.html
        │
        └───registration
            └───login.html
```

## Commands
### Run
```python manage.py runserver```
### Create Admin User
```python manage.py createsuperuser```
### Change User Password
```python manage.py changepassword [username]```

## Steps To Run
1. Create ```Super User``` using ```python manage.py createsuperuser```
1. Login to ```Admin Console``` [localhost:8000/admin](http://localhost:8000/admin)
1. Create ```General User``` using [Admin Console](http://localhost:8000/admin) and log out
1. Goto ```Polling App``` [localhost:8000](http://localhost:8000) and login using the above created ```General User``` credentials
