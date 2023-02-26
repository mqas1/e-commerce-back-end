# E-commerce Back End

[![License](https://img.shields.io/badge/License-ISC-blue.svg)](https://opensource.org/licenses/ISC)

## Description
Internet retail – or e-commerce – has been on an upward trajectory for some time now. Factoring in its resilience over the preceding years it is making more sense for traditional brick and mortar stores to improve their internet prescence with a webstore leveraging the latest technologies.

One of the key technologies required is a functioning database that will interact with the back end of the webstore. The source code in this repository contains everything a budding e-commerce business needs in those regards.

This application employs an Express.js API that is configured with Sequelize to interact with a MySQL database. The API routes perform RESTful CRUD operations.

[Walkthrough video](https://drive.google.com/file/d/1L86lsuXE5YQKUWJl2-t_xyFk8A3GbAWk/view?usp=sharing).
  
## Table of Contents
  
- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)
- [Contributing](#contributing)
- [Tests](#tests)
  
## Installation
This application requires [Node.js](https://nodejs.org/en/download/), and [MySQL](https://dev.mysql.com/downloads/mysql/). Once installed, initialise the database from the command line by ```mysql -u root -p``` and enter one's MySQL password as prompted. Then enter ```source schema.sql;```.

From the command line run the following command, ```npm i```, to install the required packages. 

Seed the database with ```npm run seed``` and start the server with ```npm start```.

## Usage

Follow these API routes for RESTful CRUD operations:

### GET Requests
```
GET /api/categories – returns all categories with their associated products

GET /api/categories/:id – returns a particular category searched by ID with its associated products

GET /api/products – returns all products with their associated categories and tags

GET /api/products/:id – returns a particular product by ID with its associated categories and tags

GET /api/tags – returns all tags with their associated products

GET /api/tags:id – returns a particular tag by ID with its associated products
```

### POST Requests
```
POST /api/categories – creates a new category in the database

POST /api/products – creates a new product in the database

POST /api/tags – creates a new tag in the database
```

### PUT Requests
```
PUT /api/categories/:id – updates a particular category in the database by ID

PUT /api/products/:id - updates a particular product in the database by ID

PUT /api/tags/:id - updates a particular tag in the database by ID
```

### DELETE Requests
```
DELETE /api/categories/:id – deletes a particular category from the database by ID

DELETE /api/products/:id – deletes a particular product from the database by ID

DELETE /api/tags/:id - deletes a particular tag from the database by ID
```

## Credits
Express.js API by [edX](https://techbootcamp.sydney.edu.au/coding/) and configured to use Sequelize to interact with a MySQL database by [Morgan Qasabian](https://github.com/mqas1). 
  
## License
This application is covered under the [ISC License](https://opensource.org/licenses/ISC):
        
        Copyright 2023 edX/mqas1

        Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.

        THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
         
## Contributing
  
The guidelines for contributing to this application can be found at the [Contributor Covenant](https://www.contributor-covenant.org/).

## Tests

Test the routes from the [Usage](#usage) section in [Postman](https://www.postman.com/downloads/) or [Insomnia](https://insomnia.rest/download).
     
---
  
*This README was made with ❤️ by the [README Generator](https://github.com/mqas1/readme-generator)*
