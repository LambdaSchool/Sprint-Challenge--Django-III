
- Link to your Djorg repo, deployed site, and a summary of your status:
    https://github.com/jamiemd/djorg
    https://mydjorg.herokuapp.com/wiki/


    - Did you reproduce the MVP apps we worked on together?
    I was able to reproduce all the mvp apps that were required. They all are at a working state but I didn't do more than what was required other than add some vision design. Some days were spent just trying to fix bugs and get everything to just work. I didn't feel like I could add any more than what was necessary because I didn't fully understand what was happening in my base code. I rewatched all 
    the lecture videos after the teacher had posted them the same day so I could go back and take notes since it was a lot of material to cover. 


    - Did you add 3rd party oauth?
    Yes, I did add 3rd party oauth just as the teacher did during the lecture so the user can sign in and create articles and their names should be attached to it.


    - How far did you get in adding your own app?
    I got as far as creating a semi functional wiki app. It doesn't have all the features of a basic wiki app. I modeled the app from the bookmark app so I was able to at least create an app that has forms where a user can enter their wiki article and save, update, and delete it. 



- Describe the design of the app you added:


    - What data/models did you write?
    I created two models. One is the wiki model that should save necessary information such as the author, title, content, date of creation, and revision date. The other model is the revision model which I am still in the process of creating. I found some code resources online for creating a wiki but I it was still difficult for me to use them because of my lack of understanding of python. I am still researching how to create the feature of saving all the revision history of an article but I'm stuck figuring out how the model will look like. 


    - What packages did you use?
    I did not use any packages other than what the teacher had us install for the previous apps. 


    - What features did you add?
    My wiki app has a page that lists all the articles that users created. If there are no articles then a user can go to the wiki creation page and add the title and content in a form. Once a user hits submit, the article will appear on the list page.Once an article is on the list, a user can click on the article title and go to the article page where a user can view the article title,author, update and revision dates, and content. Below the content are the edit wiki and delete wiki buttons. If a user clicks on the edit wiki, they are taken to a form page that has the title and content for revision. On submit, the revisions are made and once a user goes back to the article page, the article should show the update. The delete button takes the user to another page that has the article data, and once they click the delete button, that article should not show up on the article list page anymore. Unfortunately for all three: creat, edit and delete, I wasn't able to add a "success" or "fail" status when the user clicks submit or even have the page redirect to the proper page after the action. There is also a choose "author" drop down which shouldn't be on the form as an article should know by whoever is logged in who the author is. However, my app kept crashing if I removed it so I've left it in for now. 

    Learning how to use Python and Dango has been extremely enjoyable. Aaron Gallant did a great job of explaining each line of code and showing us the commands for working in the terminal, especially for someone like myself who only uses the terminal when necessary. I thought the mvp goals for each day was a good amount and we had the opportunity to take it further if we wanted. The example apps were very useful in understanding the basics of making a simple app which helped me greatly by giving me a base from where I could start my own app. Because of this experience,I want to continue furthering development of my wiki app. I could possibly make a wiki app for a specific topic such as a favorite show or cuisine. The features I would add are the revision list page, having links to other articles within one article just like Wikipedia, as well as improving the aesthetics of the app with CSS and using React for the front end. It's been a very informative three weeks learning Python and Django so I hope I'm able to have a fully functional wiki app sometime in the near future. 

 