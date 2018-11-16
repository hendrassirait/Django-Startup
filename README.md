# Django-Startup

its just my note of how to start django project in mac

1. install homebrew by typing this command in terminal, homebrew is a package manager

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

2. once you install homebrew, install python3 by typing

brew install python3

3. after that install pipenv to create a virtual environment for python, pip3 is a package manager, ist already included when you install python from homebrew

pip3 install pipenv

4. create a folder

5. on terminal, change directory to that folder

6. istall django with pipenv in that folder so you can install different environment in other project

pipenv install django==2.1

7. check if its installed correctly by typing this in terminal

ls

it should be shown these 2 filse

Pipfile
Pipfile.lock

8. go to virtual environment by typing (need to do this everytime you work on your project)

pipenv shell

9. start django project. (hello_project is the name of your project, while dot (.) in the end meand start project in this current directory

django-admin startproject hello_project .

10. after that if you type ls in terminal, you should see 2 additional file

hello_project
manage.py

11. then you can start your server by typing 

python manage.py runserver

12. if you get error, you need to migrate it first by typing

python manage.py migrate

then runserver again

13, you should see something like "Starting development server at http://127.0.0.1:8000/" in your terminal after you start server, you can copy and paste the url to your browser
