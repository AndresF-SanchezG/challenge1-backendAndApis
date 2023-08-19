# Timestamp Microservice

Build a full stack JavaScript app that is functionally similar to this: https://timestamp-microservice.freecodecamp.rocks.

This code is for a Node.js application that sets up a basic API using the Express.js framework. The application provides endpoints to handle date-related requests and return corresponding Unix timestamps and UTC strings. Here's an explanation of the code:

Importing Modules:

The required modules, express and cors, are imported to create the server and enable Cross-Origin Resource Sharing (CORS).
Initializing the Express App:

An instance of the Express app is created using express().
CORS Configuration:

CORS is enabled using the cors middleware to allow remote testing of the API.
Legacy browsers that might have issues with a 204 response are sent a 200 status.
Static File Serving:

The app serves static files located in the "public" directory. This is useful for serving client-side files like CSS, images, and JavaScript.
Basic Routing:

When a request is made to the root ("/") path, the server sends the "index.html" file located in the "views" directory.
Date Validation Function:

The function isInvalidDate(date) is defined to check if a given date is valid by comparing its UTC string representation with "Invalid Date."
API Endpoint for Date Conversion:

An API endpoint (/api/:date) is created to handle requests with a provided date parameter.
The parameter is used to create a JavaScript Date object.
If the date is invalid, it's checked if the parameter is a numeric value (Unix timestamp).
If the date is still invalid, an error response is sent.
If the date is valid, the server responds with an object containing the Unix timestamp and UTC string representation of the date.
Default API Endpoint:

Another API endpoint (/api) is defined for cases when no date parameter is provided.
It responds with the current Unix timestamp and UTC string representation.
Server Listening:

The server starts listening on the port specified in the process.env.PORT variable.
A message is logged to indicate that the server is running and listening on the specified port.
In summary, this code creates a simple Express.js application that serves static files, handles API requests related to date conversion, and responds with Unix timestamps and UTC strings. It's a basic example of building a RESTful API using Node.js and Express.js.
  
# Solution Challenge
In this challenge I tried to get as close as possible to your solution:
- Live Site URL: [Replit](https://replit.com/@AndresF-Sanchez/boilerplate-project-timestamp-3)

# Author

- Author - [@AndresF-SanchezG](https://github.com/AndresF-SanchezG)
- School - [Freecodecamp](https://www.freecodecamp.org/)
- Curse - [Timestamp Microservice](https://www.freecodecamp.org/learn/back-end-development-and-apis/back-end-development-and-apis-projects/timestamp-microservice)







