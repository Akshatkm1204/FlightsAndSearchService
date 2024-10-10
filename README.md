# Welcome to Flights Service 

## Project Setup 
- clone the project on your local 
- Execute  `npm install` on the smae path as of your root directory of the downloaded project
- Create a `.env` file in the root directory and add the following environment variable 
    - `PORT = 3000 `
- Inside the `src/config` folder create a new file `config.json` and then add the following piece of json


```
{
  "development": {
    "username": "<YOUR_DB_LOGIN_NAME>",
    "password": "<YOUR_DB_PASSWORD>",
    "database": "FLIGHT_SEARCH_db_dev",
    "host": "127.0.0.1",
    "dialect": "mysql"
  },
}


```
- Once you have added your db config as listed above, go to the src folder from your terminal and execute  `npx sequelize db:create`

`npx sequelize db:migrate`

```

## DB Design
- Airport Table
- Flight
- Airport 
- City 

- A flights belongs to an airplane, but one airplane can be used in multiple flights.
- A city has many airports, but oe airport belongs to a city.
- One airport can have many flights, but a flight belongs to one airport.
