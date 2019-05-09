Heroku Agario Server:

How do you use it?. Well its not that difficult.
Step 1: create a new heroku app with the buildpacks nodejs and php(this will be the client)

step 2: link it to this github and deploy master

step 3: go to https://YOURAPP.herokuapp.com and it should redirect to https://YOURAPP.herokuapp.com/www/index.html and show a agario client


step 4: make another app(preferably on the same pipeline) using the buildpack nodejs and deploy one of the branches below for a gamemode
teams mode : teams branch
FFA(free for all): FFA branch
Instant merge: Server Branch
Or create your own gamemode by making a new branch from FFA and editing the gameserver.ini file in the src folder


step 5: once you deployed the gameserver branch you now want to set the websocket server for the client to do so go to master branch then www/index.html and where it says freeforall1.herokuapp.com or teams1.herokuapp.com put your application name so yourapp.herokuapp.com and commit. 

step 6: Deploy the  master branch on your client application and chose the server you put your app under in index.html and have fun!
