# ecommerce-backend
A back end e-commerce site for internet retailers

## Description

This project uses npm, inquirer, MySQL, Dotenv, and Sequelize to create a backend e-commerce site for retailers. This is done by configuring a working Express.js API to use Sequelize to interact with a MySQL database. By using GET, POST, PUT, and DELETE routes, the user can choose to view all, create, update, or delete products, tags, or categories. This API was tested using Insomnia to visualize changes to each route handler and verify functionality.

<!-- Provide a short description explaining the what, why, and how of your project. Use the following questions as a guide:

- What was your motivation?
- Why did you build this project? (Note: the answer is not "Because it was a homework assignment.")
- What problem does it solve?
- What did you learn? -->

## Table of Contents (Optional)

<!-- If your README is long, add a table of contents to make it easy for users to find what they need. -->

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)
- [Badges](#badges)
- [Features](#features)
- [Tests](#tests)

## Installation

Initialization: 
Copy the SSH code within this Github Repo 
```
git clone {SSH Code}
npm init -y
npm install --save mysql2
npm install sequelize sqlite3
npm install dotenv --save
mysql -u root -p
source db/schema.sql
exit
node seeds/index.js
node server.js
```

<!-- What are the steps required to install your project? Provide a step-by-step description of how to get the development environment running. -->


## Usage

There are 8 main sections of this repository:

- [Config Folder](https://github.com/abbeydoyle/ecommerce-backend/tree/main/config) - Contains the js file enconding dotenv and sequelize functionality for connecting the database

- [DB Folder](https://github.com/abbeydoyle/ecommerce-backend/tree/main/db) - Contains the schema.sql file used for database creation

- [Models Folder](https://github.com/abbeydoyle/ecommerce-backend/tree/main/models) - Contains all fields and rules for each product, tag, and category model

- [Routes Folder](https://github.com/abbeydoyle/ecommerce-backend/tree/main/routes) - Contains JS route functions for each category, product, and tag groups, including GET, POST, PUT, and DELETE routes

- [Seeds Folder](https://github.com/abbeydoyle/ecommerce-backend/tree/main/seeds) - Contains the seeds data to populate the database upon app initialization

- [gitignore](https://github.com/abbeydoyle/ecommerce-backend/blob/main/.gitignore) - Contains all files to be ignored in the Github repository

- [License](https://github.com/abbeydoyle/ecommerce-backend/blob/main/LICENSE) - Contains the webpage license

- [ReadMe](https://github.com/abbeydoyle/ecommerce-backend/blob/main/README.md) - This file containing an executive overview of the project


Select the gifs below to be redirected to the videos demonstrating the app's funcionality

[![Screencastify VSCode demonstration](./assets/vscodescreencastify.gif)](https://drive.google.com/file/d/1J-5IYGvaGA1zNrDGdJ4okgSz4it4nXS0/view) [![Screencastify VSCode demonstration](./assets/insomniascreencastify.gif)](https://drive.google.com/file/d/160TTKoMAUlA6jp0DGju7dzQLX6wWmoHz/view)




<!-- Provide instructions and examples for use. Include screenshots as needed.

To add a screenshot, create an `assets/images` folder in your repository and upload your screenshot to it. Then, using the relative filepath, add it to your README using the following syntax:

    ```md
    ![alt text](assets/images/screenshot.png)
    ``` -->

## Credits

This webpage was built using UW Trilogy Bootcamp class materials as references.


## License

MIT License

Copyright (c) 2022 abbeydoyle

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

<!-- The last section of a high-quality README file is the license. This lets other developers know what they can and cannot do with your project. If you need help choosing a license, refer to [https://choosealicense.com/](https://choosealicense.com/). -->

---

<!-- 🏆 The previous sections are the bare minimum, and your project will ultimately determine the content of this document. You might also want to consider adding the following sections. -->

## Badges

![badmath](https://img.shields.io/github/repo-size/abbeydoyle/ecommerce-backend?color=pink&style=plastic)

![badmath](https://img.shields.io/github/issues-closed-raw/abbeydoyle/ecommerce-backend?color=pink&style=plastic)

![badmath](https://img.shields.io/github/issues-raw/abbeydoyle/ecommerce-backend?color=pink&style=plastic)

![badmath](https://img.shields.io/github/license/abbeydoyle/ecommerce-backend?color=pink&style=plastic)

![badmath](https://img.shields.io/github/commits-since/abbeydoyle/ecommerce-backend/3cafcf0/main?color=pink&style=plastic)

![badmath](https://img.shields.io/github/last-commit/abbeydoyle/ecommerce-backend?color=pink&style=plastic)

![badmath](https://img.shields.io/maintenance/yes/2023?color=pink&style=plastic)


<!-- ![badmath](https://img.shields.io/github/languages/top/lernantino/badmath)

Badges aren't necessary, per se, but they demonstrate street cred. Badges let other developers know that you know what you're doing. Check out the badges hosted by [shields.io](https://shields.io/). You may not understand what they all represent now, but you will in time. -->

## Features

This app features:

- GET routes that return all items for product, tags, and category groups
- GET 1 routes that return specified items in each group
- POST routes to add a new product, tag, or category
- PUT routes to update any product, tag, or category
- DELETE routes to delete a specified product, tag, or category



<!-- If your project has a lot of features, list them here. -->

<!-- ## How to Contribute

If you created an application or package and would like other developers to contribute it, you can include guidelines for how to do so. The [Contributor Covenant](https://www.contributor-covenant.org/) is an industry standard, but you can always write your own if you'd prefer. -->

## Tests

- Use the GET routes all product, tags, or category items listed
- Use the GET 1 route to see a specific item in each group
- Create a new product, category, or tag using the POST route, resend the API using Insomnia, and see the new information added using the respective GET 1 request for each group
- Update any product, category, or tag using the PUT routes and check that it has been updated using the GET 1 route
- Delete any item using the DELETE route with the specific ID and check it has been deleted with the GET 1 route to receive an error message that this ID does not exist



<!-- Go the extra mile and write tests for your application. Then provide examples on how to run them here. -->