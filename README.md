# Web Engineering Mini-Core assignment: Front-end
For the Mini-Core assignment, a React app was created to act as a front end. Considering I am currently still in the process of learning React, it was a good choice to continue creating new React apps to continue said process. In this project, it was particularly challenging to set up dynamic URLs for the API being used; this was done so that when running the app in a development environment local URLs were used, and when the project was deployed to Heroku the URLs of the deployed API were used. The problems that arose due to these configurations came from learning how to use environment variables (a .env file), React context, and deployment configurations so that Heroku runs the app in a production environment. Solutions for these last deployment configurations issues are explained in these commits: [Local server](https://github.com/Diego-Hiriart/Minicore-Frontend/commit/e8f19b693512f5a9b0a71f2e61e8c372bd09867c) and [Prod env, style](https://github.com/Diego-Hiriart/Minicore-Frontend/commit/5f7b271b973d14f4a8df5dbb9296826f22893e0e).

# Installing and running the React app locally
First of all, make sure you have installed Node in your computer, this will allow you to run the commands you need. Then, once you have downloaded the code, open the folder in Visual Studio Code and open a terminal, run this command in it:
```
npm install
```
That will install all the necessary dependencies (packages) needed for the React app. When the installation has completed, you can run the app with:
```
npm start
```
With that command, you will start up a development server, which will not only locally start the app in the designated port but will also reload the app whenever you save changes without needing to restart the server.\
Remember, this React app uses the API developed as a back end for this project, so you will also need to install and run that. You can find the repo here: [Web Engineering Mini-Core assignment: Back-end API](https://github.com/Diego-Hiriart/Minicore-Backend).

# Deployed web site
This React app has been deployed to Heroku, you can use it like a web site here:
  - [https://minicore-front-hiriart.herokuapp.com/](https://minicore-front-hiriart.herokuapp.com/)

# Using the web site
It is relatively simple to use the web page, but first of course, there must be a connection to a functioning API. Then, as soon as the page loads, the data corresponding to *Users* *Pass types* and *All purchased passes* will fetched from the API and displayed in the corresponding tables. To use the filtering functionality 

# Mini core functionality
The project consists of a site where parking passes can be checked, this includes viewing information about registered users, types of passes available, the passes that users have purchased, and, most importantly, a filtering functionality. When using the filter, a date must be passed, and the following is achieved:
  - By default, only filter through passes that, to the present day, have not ran out.
  - Show an estimated number of remaining passes (to the present day).
  - Calculate an estimated date on which the passes will ran out.
  - Using the selected date, filter out passes that would run out before that date.

# Contact
[hiriart.leon.d@gmail.com](mailto:hiriart.leon.d@gmail.com)
