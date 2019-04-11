## Heroku
### Dynos
Dynos are managed runtime containers with a Linux operating system.  These containers run processes that allow the code to run.
* Containerization is a mechanism for keeping running processes isolated one from another.
* Runtime containers keep code and configuration from touching another.
* Containers also provide separation between two or more dynos running identical instances of the app, accepting client requests and serving up responses.
### Slugs and Buildpacks
Slugs are compressed and pre-packaged copies of the application optimized for distribution to the Dyno manager.
When you push code to Heroku, your code is received by the slug compiler which transforms it into a slug.  Slug compiler is a collection of scripts called a buildpack that handle different languages.
### Heroku Router
Whenever a new web dyno starts up, it registers itself with the router, letting it know which application the dyno is running.   After a dyno is registered, the Heroku router begins distributing incoming requests across all the available dynos for an application, the app's "dyno formation" — that's what we call the size and number of dynos running your app.
* [HTTP Routing](https://devcenter.heroku.com/articles/http-routing)
### Heroku Add-ons
* [Heroku Add-ons](https://elements.heroku.com/addons)
### Heroku Connect
Heroku Connect is an add-on that syncs data from a Force.com database into a Heroku Postgres database and vice versa. 
* [Heroku Connect Devcenter Documentation](https://devcenter.heroku.com/articles/heroku-connect)