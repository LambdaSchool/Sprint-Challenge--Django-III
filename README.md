# Sprint-Challenge--Django-III

You've worked with Django a lot, the sprint challenge is - put it all together!
Your task is to open a PR to this repo with a file `DjangoRetrospective.md` that
answers the following questions:

- Link to your Djorg repo, deployed site, and a summary of your status:
    - Did you reproduce the MVP apps we worked on together?
    Yes
    - Did you add 3rd party oauth?
    Yes
    - How far did you get in adding your own app?
    I connected my React frontend with Django Backend. However I could not get the POST requests activated b/w frontend and backend
- Describe the design of the app you added:
    React frontend with Django Backend through rest api, db sqlite3 for persisiting data

    - What data/models did you write?
    A Task model having four fields (id, title, isDone, isDoing)
    - What packages did you use?
    django
    gunicorn
    "psycopg2-binary"
    dj-database-url
    djangorestframework
    django-allauth
    django-cors-headers
    - What features did you add?
    A task can be switched in three states (ToDo, isDoing/inprogress, isDone)
    The tasks change color acc to their state
    Todo - Red 
    In Progress - Yellow
    Done - Green

Feel free to describe both what you did build as well as what you'd like to
build with more time (be clear which is which). The main goal is an MVP that
shows you know how to build complete basic Django apps, but ideas and plans to
take it further are great and good to practice your technical writing.
With more time, I would have built a complete authentication system for an idividual to have his personal list of tasks

You can use the sprint challenge time to actually work on Djorg and get it as
far as you are able, but you do need to turn in this writing so it is suggested
you start writing by the early afternoon. We're looking forward to see what you
built - thanks for your hard work!
