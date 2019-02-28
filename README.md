# Burger app for Penn LPS Coding Boot Camp

The Burger app uses the following technologies: Node, MySql, Express, and Handelbars

Functionally, the burger app reads and manipulates data from a SQL database - either one created locally or one hosted online with the JAWSdb plugin for heroku. The connection.js file figures out whether we can go online or connect locally, and connects the DB to our orm.js file, makes the SQL data readabel for the rest of our application.  - in this case reading existing burger data, adding new burger data, or changing the burgers "eaten" status in the DB. 

Our burger.js file provides functions for reading all data from the databae, adding items, and changing data in the database (in this instance simply changin a burger from "eaten" to "uneaten").




#Running the app

If the Heroku link is still live, one can simply go to https://pacific-earth-78847.herokuapp.com/ and run things from there. 

Otherwise, one must clone the repository from https://github.com/Ignatzz/burger After doing so they will first need to run an npm install in the root directory. Then they will need to open MySQL workbench, and run first the schema.sql file then the seeds.sql file to create and populate our burgers_db. 