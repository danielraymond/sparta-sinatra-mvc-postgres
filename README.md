# Sinatra MVC Web App using PostgreSQL Database

### How to run the app:
First clone this directory from github (follow this guide if you don't know how - https://help.github.com/articles/cloning-a-repository/).

PostgreSQL must be downloaded onto your machine to run this app and a database of blog must be created. The latest version of PostgreSQL can be found here - https://www.postgresql.org/

Once downloaded you can create a database using the psql terminal by running the following in your terminal and then using the psql terminal that opens (\q exits the psql terminal.):

```
psql
CREATE DATABASE blog;
\q
```
To run the seed file that seeds the database with a posts table and data run the following command in your terminal:

```
psql -d blog -a -f seed.sql
```

To install all the required gems run the following command in your terminal (MacOS) to use the Gemfile (you must be in the **forms-and-method-overide-starter-code** directory):

```
cd forms-and-method-overide-starter-code

bundle install
```
In order to host the server for the web app locally run the following command in the forms-and-method-overide-starter-code directory.

```
rackup
```
Then go to the following address in your browser - http://localhost:9292/

The web app should load in your browser where you can view lots of examples of posts.

### Sinatra MVC Web app
In this repo is an example of a web app created using Sinatra where a restful resource of Posts has been used that can be created, read, updated and deleted.

This is an example of an app that uses the MVC architectural framework where there is a controller that processes requests from a user and responses from the server (hosted locally), a model that interacts with a PostgreSQL data base and views that are sent to the client side and are displayed in the browser.

In order to make an MVC app with your own resource follow the format but change class names and database and table names.

For an explanation of Rack look at the following guide - https://blog.engineyard.com/2015/understanding-rack-apps-and-middleware
### Documentation:

Sinatra - http://sinatrarb.com/documentation.html

PostgreSQL Guide - http://www.postgresguide.com/
