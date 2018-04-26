# Link to your Djorg repo, deployed site, and a summary of your status:

* Did you reproduce the MVP apps we worked on together?

Answer: Yes, I reproduced a todo app.

* Did you add 3rd party oauth?

Answer: Yes, I added 3rd party oauth.

* How far did you get in adding your own app?

Answer: I added graphql api and am doing the react frontend.

* Describe the design of the app you added:

Answer: The model of todo app has two fields that are title and content. I am trying to create full CRUD functionality of todo app and even plan to add more features like jwk auth and filtering function in the future.

* What data/models did you write?

Answer: Model is Todo model that contains 2 fields: title, and content.

* What packages did you use?

Answer: I added django-graphene, django-allauth, etc.

* What features did you add?

Answer: I added creating todo, displaying all the todo and graphql api for the backend. Front-end will rely on React. The front-end project will be deployed on github page whereas backend project will be hosted on heroku.

* Procedure of building Django application

Answer:

1.  setup the virtual environment for Django project, and we are using python3 and pip3 to install virtualenv, virtualenvwrapper, and pipenv.

2.  after setting up the virtual environment, we can pipenv to the virtual environment and use django-admin startproject [Project_Name] to create the main project which will have main settings.py and urls.py files.

3.  using `pipenv install` to set up the dependencies of the project.

4.  re-enter the django virtual environment to make sure all the packages are loaded.

5.  using `django-admin startapp [App_Name]` to create actual web application.

6.  in the models.py from the app folder, create the actual model data that you want to design for the application, and in the project settings.py file, register the new application which will help create the actual migration files for the model data.

7.  using `python manage.py makemigrations` and `python manage.py migrate` to create the ORM for your application so that you could play with data in the django shell.

8.  using `python manage.py shell` to get into the shell to look up the data you have.

9.  in the views.py file of the application, create the requests that will expose the data to the frontend from backend controllers.

10. in the urls.py file of the application, expose the url.

11. in the urls.py file of the project, register the urls of applicaiton so that the main project knows that the application has such urls for users to browser.

12. in the application folder, create template folder for frontend views that will interact with the backend routers which are urls and fetch data through controllers which are views.

13. after done all these, we can start the django server using `python manage.py runserver` and the default port number will be `800`.

14. now you can visualize the data in the browser and more than that is you create the admin user using `python manage.py createsuperuser` which will allow you to log in the application as administrator in the admin dashboard that is built by django and audit all the data you have.

15. you can also register your models in the application admin.py to expose the data to admin dashboard which makes it easy for you to audit the status of all the applications you have created.

16. once you are done, you could choose to deploy your whole project in the world wide web for people to look up and use. It is totally up to you.
