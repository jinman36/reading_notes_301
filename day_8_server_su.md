# Day 8

## Server Set up

### Date 10-9-2021
- Pass by value - I can do what ever I want to it - the original will not be changed
- Pass by reference - Will modify the original object

- A lot of times API's will have a finite amount of times that they will allow a server to hit it - A server can add create a buffer by caching info for this to 

- backend steps to create a server
  - npm init
  - (index.js) server.js
  - enter until is asks if that is ok - this will create a package.json to work with and install packages
- Packages to install (npm i)
  - express
  - cors - security policies
  - dotenv - env files

- Create empty file
  - touch server.js
  - touch .env
  - touch sample.env
  - touch .eslintrc.json - paste contents from class repo
  - touch .gitignore - copy contents from class repo / ensure .env is present in gitignore file


- Continue working through VS code
<!-- Boiler plate set up -->
  - server.js
    - 'use strict'
    - const express = require('express');
    - require('dotenv').config();
    - const cors = require('cors');
    const {request } = require('express')
    - const app = express();
    app.use(cors());
    <!-- set our port use to de-conflict with frontend -->
    - const PORT = process.env.PORT || 3001;


    - env file
      - PORT = 3001
<!-- Bottom of Js file -->
- app.listen(PORT, () => console.log('Listening on Port:', PORT));

  - to launch server
    - node server.js
      - this will be sttic and need to be reloaded after ever change
    - npx nodemon
      - this will allow auto update
        -  installed gloabally with 'npm i -g nodemon'

    <!--setting the root route  -->
    - app.get('/', (request, response) => {
        response.send('Greetings from the Smash server');
    })
  <!-- End of Boiler Plate -->
  const smashArr = [
    {name: 'Ness', game: 'EarthBound', rating: 'Awesome', misc: 'Stuff'},
    {name: 'Link', game: 'Legend of Zelda', rating: 'Great', misc: 'Stuff'},
    {name: 'mario', game: 'SMB', rating: 'Cool', misc: 'Stuff'},
    {name: 'Terry Bo', game: 'King of fighters', rating: 'Swell', misc: 'Stuff'}
  ];

  app.get('/allGames', getAllGames)

  function getAllGames (request, response) {
    <!-- shape response data -->
    const allGamesArr = smashArr.map(character => {
      return{name: character.name, game: character.game}
    });
    <!-- send it to the requestor (client) -->
    response.status(200).send(AllGamesArr);
  }


    - app.get('/captainfalcon', (request, response) => response.json({name: 'Captain Falcon', Game: 'F-Zero'}))

    - app.get('*', (request, response) => {
      response.status(404).send('that didn't work')
    })

<!-- This will return the character and name of game only - even though we have more information available -->

- Status codes
  - 200 - Ok
  - 300 - Further Action required
  - 400 Bad Request (404- not found)


  <!-- Back in the front end -->