# E-Commerce Back-End

## Description

For this Module 13 Challenge, the challege was to build the back end for an e-commerce site by modifying starter code. We had to configure a working Expres.js API to use Sequelize to interact with a MySQL database. The motivation for this project is that internet retail, also known as **e-commerce**, is the largest sector of the electronics industry, generating an estimated $29 trillion in 2019. E-commerce platforms like Shopify and WooCommerce provide a suite of services to businesses of all sizes. Due to their prevalence, understanding the fundamental architecture of these platforms will benefit us as a full-stack web developer. This project helped strengthen my skills with databases and routes.

## User Story

```md
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies
```


## Acceptance Criteria

```md
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia
THEN I am able to successfully create, update, and delete data in my database
```

## Installation

To use this application, please follow the link to the GitHub repository, https://github.com/thanhmhoang/ecommerce-backend. Once on the GitHub repo, click on the green "Code" button, then click "SSH" and copy the text in the box to be used as your SSH key. Next if you are on Windows, open your Git Bash, and your terminal if on Mac. Then proceed to where you would like this folder me location in your device and run the command 
The application will be invoked by using the following command:
```bash
git clone git@github.com:thanhmhoang/ecommerce-backend.git
```
Please make sure that your MySQL server downloaded and running. 

Users will also need to install the following dependencies to run the application properly, this can be done by running the following command:

```bash
npm install express sequelize mysql2 dotenv nodemon
```

If the dependencies are already listed in the package.json file provide, users can simply run the following command:

```bash
npm i
```

## Usage

To use this application, once you have completed the installation instructions, open the folder in VS code. 

Once the VS code is open, right click on the "schema.sql" file located in the "db" folder and click "Open in Integrated Terminal". Once the terminal has populated, run the following command to connect to MySQL:

```bash
mysql -uroot -p
```
Then enter your password or hit enter if you do not have a password. When you are successfully connect to MySQL, enter the following command to create your database and tables:
```bash
SOURCE schema.sql;
```

Once you have completed all of the MySQL steps, then right click on the "server.js" file and click "Open in Integrated Terminal". Once you are in the terminal, run the following command in the command line to seed data to your database so that you can tese your routes:

```bash
npm run seed
```
Then run the following command below to start the program:

```bash
npm start
```
Users can then run the application in Insomnia to GET data for each route(categories, products, or tags) as well as CREATE, UPDATE, and DELETE data in those routes.

Follow this link for a video walk-through of the application: https://youtu.be/2JfxCI7Ic4s

<img src="./assets/GET categories.png">
<img src="./assets/GET products.png">
<img src="./assets/GET tags.png">

## Credits

Jacob Nordan - Central Tutors FSF Tutor

## License

MIT License
![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)
        
Copyright (c) 2023 Thanh Hoang.
        
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
documentation files (the "Software"), to deal in the Software without restriction, including without limitation
the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions
of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO 
THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.