# crud_app 
CRUD App using NodeJs, ExpressJs, MongoDB

# Install Express generator

This app generayed by [Express generator](https://expressjs.com/en/starter/generator.html)

Install npm module express generator globally

`$ npm install -g express-generator`

`$ express`

# Installation

Get git pull from master branch.

Do `$ npm install`

Run `node server.js`

You application will run on `port: 3000`

# Dependencies

- nodejs [8.12.0](https://nodejs.org/en/download/releases/) & npm v6.4.1
- Express Js 4.16.1
- MongoDB [3.4](https://www.mongodb.com/download-center/community)

# Mongoose

Install [Mongoose](https://mongoosejs.com/docs/index.html) for schema modelling

```
$ npm install mongoose
```

# Arquiteture

`.
├── bin
├── node_modules
├── public
├── server
│   ├── cofig
│   │   └── connection.js
│   ├── controller
│   │   └── user.js
│   ├── model
│   │   └── user.js
│   ├── routes
│   │   └── user.js
│   └── service
│       └── user.js
├── views
├── package-lock.json
├── package.json
└── server.js`

# we have following folders

Config - In this folded we have maintained all the configuration related files. Here, we have used MongoDB connection in connection.js file.

Routes - In this folder have maintained all the API routings. From routing, we will access the controller file.

Controller - In this folder, we have handled the all the logic and queries for API request and here only we will give response for API call with status code and response object.

Service - In this folder, we have maintained all the MongoDB query executions.

Model - In this folder, we have maintained all the mongoose model.

# List of route paths

GET:    /api/users/user/:username

POST:     /api/users

PUT:     /api/users/updatebyid

PUT:     /api/users/update

DELETE: /api/users/delete

# Tutorial 

- https://scotch.io/@vigneshsithirai/basic-crud-operation-with-nodejs-express-and-mongodb