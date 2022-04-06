# REST API

This application is a small, self contained, in-memory REST app.

## Installation

To initialise the project you will need to install several dependencies, open up a terminal from the repo directory and run the command:

~~~ bash
$ npm install
~~~

## Running the application

In order to run the application, from your git bash terminal run:

~~~ bash
$ npm start
API Listening on http://localhost:8080
~~~

## Stopping the application

In order to stop the application from the git bash terminal that is running the server press ``CTRL`` + ``C``

## Functionality

### ENDPOINTS

#### CREATE

``POST`` endpoint at ``http://localhost:8080/create`` 

``Content-type:application/json``

example data:
~~~
{
    name : "example product", 
    description : "this is an example", 
    price : 9.99
}
~~~

#### READ

``GET`` endpoint at ``http://localhost:8080/read``

``GET`` endpoint at ``http://localhost:8080/read/:id``

#### UPDATE

``PUT`` endpoint at ``http://localhost:8080/update/:id``

``Content-type:application/json``

example data:
~~~
{
    name : "updated product", 
    description : "this product has been updated", 
    price : 999.99
}
~~~

#### DELETE

``DELETE`` endpoint at ``http://localhost:8080/delete/:id``

### IN BROWSER

In order to interact with this application through a browser navigate to ``http://localhost:8080/`` while the application is running.

The static content is stored in the ``/public`` directory.