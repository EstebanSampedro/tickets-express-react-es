# Parking tickets (CREDITS: Luis Corales)
## Objective
Replicate a Mini-Core project using a selected framework, implement the project locally and deploy it online
- Heroku deployment: https://tickets-express-react-es.herokuapp.com/

## GitHub replicated
https://github.com/LuisCoralesM/tickets-express-react

Made with React and Express

## Core project

The project consists of two apps, the backend API and the frontend. The backend has the following endpoints: 

- /api/health, GET: Just returns "ok" to check the API status.
- /api/people, POST, a date as body: Filters the people by its expiry ticket date using the passed date inserted in the client app. 
- /api/people, GET: Returns all the people data registered.

Using the web app, you could look at the whole registry of people that have bought tickets, and you could filter them by passing a date, which will return all the people with a ticket expiry date later than the date inserted. This will gather all the people data including how many tickets the have remaining until today (the date when fetched). It wont print the people with 0 or less tickets remaining.

---

## Development

Commands to start the backend side:

```
$ cd server
$ npm install
$ npm run dev
```

And to run the frontend using another terminal:

```
$ cd ../client
$ npm install
$ npm start
```
