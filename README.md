# Simple API Timestamp Microservice

## Versions

Create a file named `.env` in the root directory. This file should contain:

```
MONGO_URI=mongodb://localhost:27017/clementinejs
PORT=8080
APP_URL=http://localhost:8080/
```

### Starting the App

`node server.js` 

### Heroku app

timestamp-api-imadmk.herokuapp.com

### Using this app

     User stories:

        1) I can pass a string as a parameter, and it will check to see whether that string contains either a unix timestamp or a natural language date (example: January 1, 2016)

        2) If it does, it returns both the Unix timestamp and the natural language form of that date.

        3) If it does not contain a date or Unix timestamp, it returns null for those properties.

Example usage:
https://timestamp-api-imadmk.herokuapp.com/December%2015,%202015
https://timestamp-api-imadmk.herokuapp.com/1450137600
Example output:
{ "unix": 1450137600, "natural": "December 15, 2015" } 