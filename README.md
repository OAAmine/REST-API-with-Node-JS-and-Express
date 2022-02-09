# REST-API-with-Node-JS-and-Express
A basic patient file management system using REST API

npm init 
accept all the default settings 

install express module
let our API easily accept web requests 
npm install express

parse the body of api requests
npm install body-parser

automatically restart server when saving the file (optional)
for windows : Set-ExecutionPolicy Unrestricted (allows the execution of scripts might wanna run it with admin privilieges)
npm install nodemon -g

Since your web browser only sends GET request when typing the localhost followed by
the port number you specified (3000 in my code), i advise you to use something like 
postman which is a very intuitive app that let's send http methods of your choosing

For simplicity's sake, i used a hash table instead of a real world example which would be a database 
holding the patients information
