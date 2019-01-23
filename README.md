
# EchoJS Scraper 

## Created by Christie Byrne

### This is a full stack JavaScript application that uses NPM packages (Express, Express-Handlebars, Body Parser, Morgan, Mongoose, Request and Cheerio), Handlebars, database storage, and styling with CSS. The application allows the client to interact with a server to submit and update data using POST and PUT requests. The application employs a simple client/server full-stack approach, with a front end (HTML-Handlebars, CSS), middleware (Express, Body-parser) and back end (Mongoose models). 

## Purpose
This is aweb app that lets users view and leave comments on the latest posts. The client can scrape headlines and links from EchoJS and save the articles in a database. They can also delete saved articles, make notes on specific articles, and delete those notes.

### Scraping
The application uses "request" and "cheerio" for scraping the EchoJS website. The articles scraped are compared to the ones in the database, and if the articles hasn't already been stored, it is put into an object which is rendered on the "/scrape" route with the help of the "express-handlebars" npm package. Both the scrape page and the Saved Articles page display links to the associated articles so that the user may check out the full articles before saving or writing a comment.

### Saving Articles and Commenting
The articles are saved to the database with the help of the Mongoose NPM (an object modeling tool designed to work in an asynchronous environment). 
This application uses Article and Note models with the Article model containing an array "note" that stores the ObjectIds of any associated Note. 
From the Saved Articles page, the client can delete an article from the database or navigate to the article's Note/Comment page in order to see any associated notes/comments or to make a comment. The data on all routes is redered with "express-handlebars". A client can also create a note or read a comment by navigating to the "/articles/_id" route.

## Try it out here! https://mongooooooose.herokuapp.com/

## Built With:
HTML
CSS
JavaScript
jQuery Library
JSON
Bootstrap CSS Library
Bootstrap JavaScript Library
Node.js
Express.js
Handlebars.js
Cheerio
Request
Body Parser
Morgan
MongoDB
Mongoose
GitHub
Heroku