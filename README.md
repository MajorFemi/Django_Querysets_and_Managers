# Django_Querysets_and_Managers
A QuerySet represents a collection of objects from your database. It can have zero, one or many filters. Filters narrow down the query results based on the given parameters.



We’ll be building more features for our URL shortener service.

We want users of our API to view all active links. We also want to provide users with an endpoint to view Links created during the week.

Create a new file, managers.py in your links app folder. Replace the content of links/managers.py with this starter file https://github.com/TobeTek/Zuri/blob/main/starter-files/Querysets-and-Managers/managers.py  

 

Add the following attributes to your Link model in links/models.py

objects = models.Manager()

public = ActiveLinkManager()

 

On to the views. Copy the ActiveLinkView and RecentLinkView from  https://github.com/TobeTek/Zuri/blob/main/starter-files/Querysets-and-Managers/views.py to links/views.py.

 

Add the following new URL paths in links/urls.py.

path("active/", ActiveLinkView.as_view(), name=’active_link’)

path("recent/", RecentLinkView.as_view(), name=’recent_link’)


Note: 
Level = "Beginner"
Enjoy! 

