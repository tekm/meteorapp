# Meteor App - Keela
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)
> An app using the MeteorJS framework, with login, registration, teams & more!

## Table of contents
* [General info](#general-info)
* [Screenshots](#screenshots)
* [Technologies](#technologies)
* [Setup](#setup)
* [Features](#features)
* [Status](#status)
* [Inspiration](#info-for-keela)
* [Contact](#contact)

## General info
This project was an assigment from Keela to complete a set of tasks with a given UI. I was instructed
to create an application using the MeteorJS framework, with a front end using Blaze. The database used is
MongoDB.

## Screenshots
![Screen1](./img/screenshot1.png)
![Screen2](./img/screenshot2.png)
![Screen3](./img/screenshot3.png)

## Technologies
* MeteorJS - version 1.8.0.2
* Heroku - version 7.22.4
* MongoDB - version 4.0.6@community
* HTML, CSS, JavaScript

## Setup
```
For Mac: curl https://install.meteor.com/ | sh
brew tap heroku/brew && brew install heroku
brew tap mongodb/brew && brew install mongodb-community@4.0
git clone git@github.com:tekm/meteorapp-keela.git
cd meteorapp-keela
```
Or Use Heroku Deploy Button

Demo: https://meteorapp-keela.herokuapp.com/

## Features
* Login Page with Google OAuth Login & Twitter OAuth Login
* Registration Page with Google OAuth Login & Twitter OAuth Login
* User Page with email & name
* Teams page with the ability to view, create, search for users, and add to team

## Status
Project is: _in progress_
May use circleci or travisci, deciding

## Info For Keela
a. General flow of how to use the app\
You are first directed to the splash page, the base index page before being directed to login or register. You are able to login/register with an email address, or by using Google OAuth2/Twitter OAuth2 to access your basic profile data to create a user.
After login/registering, you are redirected to your User Profile. From your user profile you have the ability to update your first name, last name, email address, and teams you are on. 
There is a tab for teams. Selecting this tab allows for you to see the various teams on the platform, what users are on what teams, make a new team, and search for users.


b. How you structured the data\
The data is structured as follows. This allows for a nice hierarchy, that is clean and easy to follow. All functions are broken up into their respective folders.

```
| bar = tree structure
- dash = folder
_ underscore = file

Meteorapp-keela
|
|---client
|      |_______ main.css
|      |_______ main.html
|      |_______ main.js
|
|---server
|      |_______ main.js
|      |_______ init.js
|      |_______ publish.js
|
|---imports
|      |---ui
|      |   |_______ task.js
|      |   |_______ body.js
|      |
|      |---ui
|          |_______ tasks.js
|
|---collections
|        |_______ users.js
|        |_______ teams.js
|
|---lib
|    |_______ routes.js
|
|---tests
|    |_______ main.js
|
|---node_modules
|
|___package-lock.json
|
|___package.json
|
|___README.md
|
|___app.json

```
\
c. What was challenging, what you struggled with\
I've never used MeteorJS before, so I had to learn how to use it, what the common layouts of file structure are, benefits to using it. A big part of using MeteorJS is templating and real time updating. It's fast, easy to learn, and has good packages to make templating your site incredibly easy.


d. What you would like to implement or work on if you had more time\
If I had more time I would add more functionality to user roles, and what you can do with a team. I would give teams certain capabilities, such as having access to certain commands/files. User roles would allow for only certain users to add/delete teams/files.

## Contact
Email: logan.kane1@gmail.com\
[github](github.com/tekm)
