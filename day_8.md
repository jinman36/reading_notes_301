# Day 8

## Into the backend!

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


- Continue working through VS code
<!-- Boiler plate set up -->
  - server.js
    - 'use strict'
    - const express = require('express');
    - require('dotenv').config();
    - const cors = require('cors');
    - const app = express();
    <!-- set our port use to de-conflict with frontend -->
    - const PORT = process.env.PORT || 3001;


    - env file
      - PORT = 3001
<!-- Bottom of Js file -->
- app.listen(PORT, () => console.log('Listening on Port:', PORT));
  <!-- End of Boiler Plate -->

  - to launch server
    - node server.js
      - this will be sttic and need to be reloaded after ever change
    - npx nodemon
      - this will allow auto update
        -  installed gloabally with 'npm i -g nodemon'

    
