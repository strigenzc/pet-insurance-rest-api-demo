# Pet Insurance REST API Demo

A demo application that runs an API server and database locally.  
Only the health check endpoint has been implemented.  
Other endpoints will be implemented in the Future Associates API session.  

---

## Dependencies

- node  
- npm  
- mongodb-community  

install brew: https://brew.sh/  

install dependencies via brew:

`brew install node`  
`brew tap mongodb/brew`  (migrated distribution from custom tap)  
`brew install mongodb-community`  
`brew install npm`

if issue installing or updating npm: https://flaviocopes.com/npm-fix-missing-write-access-error/

Note: If you still have the old mongodb installed from homebrew-core:  
`brew services stop mongodb`  
`brew uninstall homebrew/core/mongodb`

---

## Generate Node modules
Required packages (and their dependencies) must be installed locally with the following command.  
These are defined in package.json  
`npm install`

---

## Run Database Server

To start the mongodb server locally run:
`brew services start mongodb/brew/mongodb-community`  

To stop the server:
`brew services stop mongodb/brew/mongodb-community`  

## Run API Server

To start the API server locally run:  
`npm run start`

The server runs until stopped, by cancelling execution of the command.

Hit the health check endpoint via browser (or postman) at:  
http://localhost:3000/pets