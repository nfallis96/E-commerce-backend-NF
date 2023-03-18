# E-Commerce Back End

GitHub Repository: https://github.com/nfallis96/E-commerce-backend-NF


## Table of Contents

* [Description](#description)  
* [Demo](#demo)  
* [Usage Instructions](#usage-instructions)  
* [Code Examples](#code-examples)  
* [Technologies Used](#technologies-used)    
* [License](#license)  

## Description

The purpose of this project was to build the back end for an E-commerce site. It works by configuring an express.js API to use sequelize to interact with a MySql database.

## Demo

I can't upload a demo because the mysql password for my computer is not working. 

## Usage Instructions

To use this application, follow these steps (mysql is required):
1. Clone this repository.
2. Find this repository in your terminal and run ```npm install``` to install the required dependencies.
3. To start the database type ```mysql -u root -p``` in your terminal and enter your password. Then in the mysql shell, enter ```source ./db/schema.sql```
4. Exit mysql with ```quit``` on the terminal.
5. In your terminal run ```npm run seed```.
6. You can then test the applications routes with a tool like Insomnia or Postman.

## Code Examples

This is an example of how it imports sequelize connection

```js
const app = express();
const PORT = process.env.PORT || 3001;

app.use(express.json());
app.use(express.urlencoded({ extended: true }));
app.use(routes);
```

This example shows how the application syncs sequelize models to the database

```js
app.listen(PORT, () => {
  console.log(`App listening on port ${PORT}!`);
});
```

## Technologies Used

![JavaScript Badge](https://img.shields.io/badge/Language-JavaScript-yellow)
![Mysql Badge](https://img.shields.io/badge/Database-MySql-informational)
![Node.js Badge](https://img.shields.io/badge/Environment-Node.js-red)
![Express Badge](https://img.shields.io/badge/NPM-Express.js-green)
![Sequelize Badge](https://img.shields.io/badge/NPM-Sequelize-important)
![Dotenv Badge](https://img.shields.io/badge/NPM-dotenv-blueviolet)
![License Badge](https://img.shields.io/badge/License-MIT-blue)
## License

MIT License

Copyright (c) 2023 Nicole Fallis

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
