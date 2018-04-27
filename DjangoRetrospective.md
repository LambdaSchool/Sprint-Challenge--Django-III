1. Here is a link to my djorg repository: https://github.com/kd798529/djorg
   Here is a link to my deployed djorg heroku site: https://djorgkwaku.herokuapp.com/
   	The Djorg Project was contains three apps bookmarks, notes and a personal message app called konkonsah(konkonsah is the Twi word for gossip). I have not added a 3rd party oauth to the project. I have created models and made migrations to the konkonsah app.

2. The konkonsah messaging app included the following model: 
```class Message(models.Model):
    id = models.UUIDField(primary_key=True, default=uuid4, editable=False)
    message = models.TextField(blank = True)
    created_at = models.DateTimeField(auto_now_add=True)
    last_modified = models.DateTimeField(auto_now=True)
    sender = models.ForeignKey(User, related_name="recipient", on_delete=models.CASCADE)
    recipient = models.ManyToManyField(User)```
    The sender and reciepient field contained a foreign key which showed a one to one and many to many relation ship.
    This will allow a group messaging function in addition to a regular messaging function.
    Another additional feature that will be added will be the fuction which can tell if a message has been read or not. 
    I am anticipating creating a template in which i will apply the html web stockets which is discribed on this page: https://www.tutorialspoint.com/html5/html5_websocket.htm. Theres a great deal of tools on https://socket.io/get-started/chat/ looks promising as a way to create the konkonsah app.