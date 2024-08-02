USER REGISTRATION AND LOGIN SYSTEM

I completed the user registration and login system using python django in the context of visual studio code.

SETUP AND EXECUTION STEPS

step 1

	create a new project directory and open in visual studio code.

step 2

	create a virtual environment
	
	python3 -m venv env
	
step 3

	Activating the virtual environment
	
	. env/bin/activate
	
step 4

	Install django
	
	pip install django

step 5

	Create the django project
	
	django-admin startproject project
	
step 6

	Enter into the project
	
	cd project
	
step 7

	create the django project
	
	python manage.py startapp app
	
code explaining and step 8

	Register the app
	
	Settings.py>Installed apps[
				'app',
				]
				
step 9 

	Create static and templates folders
	
	static folder will contain static files(like image,textfiles,css or javascript files,etc)..
	Templates folder contain dynamic files like HTML files
	
step 10

	set static directories and template directories
	
	settings.p>import os

step 11

	create templates
	
	login.html,register.html,home.html
	with css and javascript using the code
	
	<link rel="stylesheet" href="/static/css/style.css">
	<script src="/static/js"></script>
	
step 12

	set urls of project and app
	
	project>urls.py  from django.urls import path,
	include
	
	urlpatterns=[
	path('admin/',admin.site.urls),
	path('',include('home.urls'),
	]
	
	app>urls.py  from django.urls import path,
	include
	from django.contrib import admin
	from app import view
	urlpatterns=[
	path('',view.login,name='app');
	]
	
step 13

	define and render URLs
	
	urls.py>from django.shortcuts import render
	def login(request)
		return render(request,'login.html'{})
		
step 14

	create superuser
	
	python manage.py create superuser
	
step 15 

	Run migration
	
	python manage.py makemigrations
	python manage.py migrate
	
step 16 

	Run project
	
	python manage.py runserver
	
	
HOSTING

To hosting the django project

	copy the folder into computer and open with visual studio code
	Activate the environment
	  . env/bin/activate
	  
	Run project
	  python manage.py runserver
	
