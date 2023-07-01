# Setting up Auth0

## Create Backend Application

* Under Applications > Applications, create a new application with the following settings:
    * Name: `Project Management Backend`
    * Application Type: Regular Web Application
    * Allowed Callback URLs: `http://localhost:8012/login/oauth2/code/auth0`
    * Grant Types: Authorization Code, Refresh Token, Implicit, Client Credentials

## Create a Frontend Application

* Under Applications > Applications, create a new application with the following settings:
    * Name: `Project Management Frontend`
    * Application Type: Single Page Application
    * Allowed Callback URLs: `http://localhost:3000`
    * Allowed Logout URLs: `http://localhost:3000`
    * Grant Types: Authorization Code, Refresh Token, Implicit

## Create an API

* Under Applications > APIs, create a new API with the following settings:
    * Name: `Project Management`
    * Identifier: `projectmanagement`
    * Signing Algorithm: `RS256`
* Under Permissions tab of the API, create the following permissions:
    * `read:company`
    * `write:company`
    * `read:project`
    * `write:project`
    * `read:project`
    * `write:project`
    * `update:project`
    * `delete:project`
* Under the Machine to Machine Applications tab, Authorize the Backend Application created above to access the API and
  assign the permissions created above.
