# Timestamp Microservice

Build a full stack JavaScript app that is functionally similar to this: https://timestamp-microservice.freecodecamp.rocks.

Fulfill the below user stories and get all of the tests to pass. Use whichever libraries or APIs you need. Give it your own personal style.

# Targets

- You should provide your own project, not the example URL.
- Waiting:A request to /api/:date? with a valid date should return a JSON object with a unix key that is a Unix timestamp of the input date in milliseconds (as type Number)
- Waiting:A request to /api/:date? with a valid date should return a JSON object with a utc key that is a string of the input date in the format: Thu, 01 Jan 1970 00:00:00 GMT
- Waiting:A request to /api/1451001600000 should return { unix: 1451001600000, utc: "Fri, 25 Dec 2015 00:00:00 GMT" }
- Waiting:Your project can handle dates that can be successfully parsed by new Date(date_string)
- Waiting:If the input date string is invalid, the API returns an object having the structure { error : "Invalid Date" }
- Waiting:An empty date parameter should return the current time in a JSON object with a unix key
- Waiting:An empty date parameter should return the current time in a JSON object with a utc key
  
# Solution Challenge
In this challenge I tried to get as close as possible to your solution:
- Live Site URL: [Replit](https://replit.com/@AndresF-Sanchez/boilerplate-project-timestamp-3)

# Author

- Author - [@AndresF-SanchezG](https://github.com/AndresF-SanchezG)
- School - [Freecodecamp](https://www.freecodecamp.org/)
- Curse - [Timestamp Microservice](https://www.freecodecamp.org/learn/back-end-development-and-apis/back-end-development-and-apis-projects/timestamp-microservice)







