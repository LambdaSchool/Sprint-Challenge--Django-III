Repo: https://github.com/jessehood/djorg/  
Heroku: https://djorg-jh.herokuapp.com/

I did the MVP of the apps that we worked on and added oauth.
However, I forgot to go back to the Notes app and add forms to actually create/view notes.  
For my own app, I created a file uploader. The user can only see the files that he has uploaded 
and the files are saved with a UUID name to make it difficult to guess the URL for another user's file.
I used the "download" HTML5 tag to change the name of the file when the user actually goes to download it. 
It works locally, but unfortunately I could not figure out why Heroku was not properly serving uploaded files with the limited amount of time we have. 
  
As for the design of the app, I just used a model with a FileField to store a file linked to a user. I tried to keep it simple. 
I did not add any additional dependencies on top of what we have already added to the project. 
  
I feel that I could have done more with this project if it was done earlier in the curriculum. 
Having to juggle creating a resume/linkedin, working on the personal project, and working on this project with the added stress of Lambda Labs coming up and the inevitable job search made this project difficult to work on.