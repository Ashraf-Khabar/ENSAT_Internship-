ENSAT Internship Application
============================

<img src="https://img.shields.io/badge/Made%20by-Achraf%20Khabar-blue" alt="made by Achraf khabar"> <img src="https://img.shields.io/badge/Made%20by-Kaouthar%20bouslim-blue" alt="made by Kawtar Bouslim"> <img src="https://img.shields.io/badge/Made%20by-Nahid%20Chaoui-blue" alt="made by Nahid Chaoui"> <img src="https://img.shields.io/badge/Made%20by-Abir%20el%20bouzayani-blue" alt="made by Abir el bouzayani"> <img src="https://img.shields.io/badge/Framed%20by-Mr.%20Hassan%20Badir-green" alt="Framed by Mr. Hassan Badir">

<p align="center">
  <img src="https://cdn.freebiesupply.com/logos/thumbs/2x/nodejs-1-logo.png" alt="Node.js" height="70">
  <img src="https://cdn.worldvectorlogo.com/logos/express-1.svg" alt="Express.js" height="70">
  <img src="https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg" alt="React.js" height="70">
  <img src="https://www.mysql.com/common/logos/logo-mysql-170x115.png" alt="MySQL" height="70">
  <img src="https://sequelize.org/v5/manual/asset/logo-small.png" alt="Sequelize ORM" height="70">
 </p>

Introduction
------------

This web application connects students from ENSAT (Ecole Nationale des Sciences Appliquées à Tanger) with companies for internships. Companies can create an account and add internship offers, allowing ENSAT students to apply for the positions. The app is built using Node.js, React.js, Express.js, Sequelize, and MySQL.

Features
--------

-   Connects ENSAT students with companies for internships
-   Companies can create accounts and add internship offers
-   Built with Node.js, React.js, Express.js, Sequelize, and MySQL

Requirements
------------

-   Node.js
-   React.js
-   Express.js
-   Sequelize
-   MySQL

Installation
------------

1.  Clone the repository to your local machine
2.  Navigate to the `server` directory using your terminal/command prompt
3.  Install the required dependencies by running `npm install`
4.  Start the Node.js server by running `npm start`
5.  Navigate to the `client` directory using your terminal/command prompt
6.  Install the required dependencies by running `npm install`
7.  Start the React development server by running `npm start`

Usage
-----

1.  Start the Node.js server by running `npm start` in the `server` directory, le fichier `index.js` : 
  ```js 
    import express from "express";
    import dotenv from "dotenv";
    import cookieParser from "cookie-parser";
    import cors from "cors";
    import db from "./config/Database.js";
    import router from "./routes/index.js";
    import * as bodyParser from "express";
    dotenv.config();
    const app = express();

    app.use(cors({ credentials:true, origin:'http://localhost:3000' }));
    app.use(bodyParser.urlencoded({ extended: false }));
    app.use(bodyParser.json());
    app.use(cookieParser());
    app.use(express.json());
    app.use(router);

    app.listen(5000, ()=> console.log('Server running at port 5000'));
  ``` 
3.  Start the React development server by running `npm start` in the `client` directory
4.  Open your browser and navigate to [http://localhost:3000](http://localhost:3000/)
5.  Companies can create an account and add internship offers, and students can apply for positions.

Contribution
------------

Feel free to fork this repository and make contributions.

License
-------

This project is licensed under the MIT License.
