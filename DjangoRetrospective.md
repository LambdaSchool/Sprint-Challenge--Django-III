## [Djorg Repo](https://github.com/adamfetters/djorg)

I was able to reproduce all the MVP apps and get them to run locally. Unfortunately I could not get them to run successfully on deployment. I did add in the 3rd party oAuth including Github, but did not add any other 3rd party sites.

I did add in graphql, but only basics for testing to see if I could even get it installed. I was successfully able to use the graphql tool to display data in the browser. I can see this as being a real advantage in the future. 

As far as the progress on my own blog app, I was able to setup the admin area to add blogs to the logged in user, display the last 10 latest posts, and include links from each post title to a details page of the corresponding blog. Unfortunately the details page was not able to be found. I did have it to where it would show the details page, but no details, so I tried some different configurations and am now getting a 404. I will continue to work on this to see where the problem lies.

As far as the models for my blog app, I had title, body, and created_at(which was set the the default time of now). I did have a model for comments, but after running into some issues, I scrapped the existing app I had and started over to make cleaner more concise code. 

I also added an internal class method of str to return the title on the back-end in admin rather than have it display "Object1", "Object2", etc. It now displays the actual title of the post. 

For the most part I used the core Django packages , but there were a few I found necessary to implement. One being django decouple: This was used for the settings parameters , allowing project settings, and instances of the project (for deployment), to be separated from the source code.

I also installed the django rest framework as a toolkit to make restful apis, but didn't get around to connecting the react front end like I wanted. I plan to do that this weekend though. Along with that was the djoser package that provides the django rest framework views to handle registration, login logout, password reset, and account activation, working with custom models.

There were a few other packages, but as most of them related to deployment, and I was unable to do that, I will bare you the details. 

I plan to really get deep into Django this weekend and would like to 1) get the blog fully functioning, 2) Turn it into more of a social network type app, and 3) get it successfully deployed. There are a lot of modules I have come across that seem to make things a lot easier, and as Django allows a person to get up and running quickly, there seems to be a lot of different ways to do things, and I want to get a good workflow.
