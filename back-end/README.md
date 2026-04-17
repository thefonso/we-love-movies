# weLoveMovies
Backend code that displays reviews of movies

## Installation

1. Fork and clone this repository.
1. Run `cp ./back-end/.env.sample ./back-end/.env`.
1. Update the `./back-end/.env` file with the connection URL's to your PostgreSQL database instances.
1. cd back-end
1. npx knex migrate:latest <--run all migrations
1. npx knex migrate:rollback <--roll them all back if needed
1. npx knex migrate:list <-- see who is pending
1. npx knex seed:run <-- seed DB
1. (Note for prod: NODE_ENV=production npx knex seed:run)
1. Run `cp ./front-end/.env.development ./front-end/.env`.
1. You should not need to make changes to the `./front-end/.env` file unless you want to connect to a backend at a location other than `http://localhost:5000`.
1. Run `npm install` to install project dependencies.
1. Run `npm run start:dev` to start your server in development mode.

## Running Tests

This project includes a set of tests that can be run using the command line. To run all the tests use the following commands:

- npm test 

### GET /movies

Making a `GET` request to `/movies` will return all movies.

