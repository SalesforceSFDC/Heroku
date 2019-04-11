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
