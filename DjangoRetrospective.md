# Django Retrospective

### Links

- Djorg Repo: https://www.github.com/williamantony/djorg
- Deployed Site: https://djorg-app.herokuapp.com

### Summary 

The project **Djorg** consist of 3 apps,
1. Bookmarks App
2. Notes App
3. Storage App

The project is deployed to Heroku and it is live at https://djorg-app.herokuapp.com.

**Exception**: *Heroku* prohibits the persistence of files uploaded, meaning the uploaded file will get deleted as soon as it receives. 
[Explanation by Heroku](https://help.heroku.com/K1PPS2WM/why-are-my-file-uploads-missing-deleted).

**Solution**: Use another file hosting provider such as Amazon Web Services.

---

#### Did you reproduce the MVP apps we worked on together?

Yes, I reproduced *Storage App*

#### Did you add 3rd party oauth?

I implemented third-party oauth using *django-allauth*. Only Github is added as oauth provider.

#### How far did you get in adding your own app?

I completed the new app and deployed to the live server.

#### Describe the design of the app you added:

The app is designed to receive files (mainly in image format) and save it in storage.


#### What data/models did you write?

I wrote a model for *File*, which have the following fields:
- id - primary key
- title - name/description
- upload - user uploaded file
- created_at - timestamp
- last_modified - timestamp


#### What packages did you use?

No additional packages were necessary to implement *Storage App*.
However, some packages that were common to other apps are:
- django-allauth
- django-bootstrap4
- djangorestframework
- graphene-django

#### What features did you add?

I added the following features:
1. Oauth based user authentication
2. File Upload using FileInput() field in Django
