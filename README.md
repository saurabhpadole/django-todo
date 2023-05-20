# django-todo
A simple todo app built with django

![todo App](https://raw.githubusercontent.com/shreys7/django-todo/develop/staticfiles/todoApp.png)
### Setup
To get this repository, run the following command inside your git enabled terminal
```bash
$ git clone https://github.com/shreys7/django-todo.git
```

# For setting up the virtual envrionment in vs code:
meaning of virtual environment: to run the project in a isolated environment where we need some specific versions of the software like for some applications we need python 3.10.
other project or app will need different versions of the software, so we will run that in other virtual environment.


To install virtual environment in vs code for windows:

requirements:
1. python should be installed on windows
2. install the extention for python in vs code

set the terminal to "cmd", do not set it to powershell

now, go to vs code
open the folder which has your project
change your directory to project/repo folder
open terminal on vs code
enter this command : python -m venv <path of you project>\venv   ----> here last "venv" is the name of the environment that you want to create
on terminal : .\venv\scripts\activate			after firing this, environment name will appear in brackets (venv) like this.


  
You will need django to be installed in you computer to run this app. Head over to https://www.djangoproject.com/download/ for the download guide

Once you have downloaded django, go to the cloned repo directory and run the following command

$ cd django-todo

$ pip install django

```bash
$ python manage.py makemigrations
```

This will create all the migrations file (database migrations) required to run this App.

Now, to apply this migrations run the following command
```bash
$ python manage.py migrate
```

One last step and then our todo App will be live. We need to create an admin user to run this App. On the terminal, type the following command and provide username, password and email for the admin user
```bash
$ python manage.py createsuperuser
```

That was pretty simple, right? Now let's make the App live. We just need to start the server now and then we can start using our simple todo App. Start the server by following command

```bash
$ python manage.py runserver
```
for Dockerfile creation:
$ pip freeze > requirements.txt

$ git checkout -b feature/deploy-app
  
$ git add .
  
$ git commit -m "added requirements"
  
$ git push origin feature/deploy-app
  
Once the server is hosted, head over to http://127.0.0.1:8000/todos for the App.

Cheers and Happy Coding :)
