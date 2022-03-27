# 13 Object-Relational Mapping (ORM): E-Commerce Back End

## Link to GitHub Repo
[Link to GitHub Repo](https://github.com/MiinoSil/13-NGO-ORM-ECOM-BAKEND-GIT-HWK)

## Description
To better understand ecommerce and the backend, this is backend app built using node.js and mysql. Function is to keep product database, set up relationship between different database tables, and modify the backend using an app like INSOMNIA. 

## NPM requirements
```
[MySQL2](https://www.npmjs.com/package/mysql2) 

[Sequelize](https://www.npmjs.com/package/sequelize) 

[dotenv](https://www.npmjs.com/package/dotenv)

[express](https://www.npmjs.com/package/express)
```

NPM should be listed under package.json dependencies to make install easier

Run the following code in terminal or command-line to install packages if package.json checks out:
```
npm install
```

## Usage
Make sure .env is setup with mysql user and password

In MySQL shell,
SOURCE the schemal.sql located in db folder to create the ecommerce_db

Run the following code to seed the database:
```
npm run seed
```

Run the following code to start the server:
```
npm start
```

Use a backend app like insomnia to listen in on localhost to view api. 
## Video Walkthrough by Andrew
![GIF demo of running mysql to SOURCE schema.sql and "npm run seed" to seed the ecommerce_db](./Assets/mysql-schema-seed-demo.gif)

[DEMO(above) demonstrating 'npm install', SOURCE schema.sql in mySQL shell to create ecommerce_db, then seeding with data by command line 'npm run seed'.](https://drive.google.com/file/d/1cS2YEIAD77cr60aeSxdXkfi1TwDf582p/view)


![GIF demo starting server, using insomnia to access api, then GET categories, products, and tags](./Assets/start-server-GET-categories-products-tags-demo.gif)

[DEMO(above) starting server, using insomnia to access api, then GET categories, products, and tags](https://drive.google.com/file/d/1qUtHpfnc0xXUCFVwE8-JBBJqxPriK7lb/view)


![GIF demo searching for single item in api by primary key id for categories, products, and tags](./Assets/GET-one-item-by-id-categories-products-tags-demo.gif)

[DEMO(above) searching for single item in api by primary key id for categories, products, and tags](https://drive.google.com/file/d/17zvUQd6-t9igQ9rJZEL37-oYmVrik5Oi/view)


![GIF demo POST, PUT, DELETE for categories, products, and tags](./Assets/POST-PUT-DELETE-categories-products-tags-demo.gif)

[DEMO(above) POST, PUT, DELETE for categories, products, and tags](https://drive.google.com/file/d/1cpcZsawAWBmThNw_aTkhb9YGTDRd5CJv/view)
## Your Task

Internet retail, also known as **e-commerce**, is the largest sector of the electronics industry, generating an estimated $29 trillion in 2019. E-commerce platforms like Shopify and WooCommerce provide a suite of services to businesses of all sizes. Due to their prevalence, understanding the fundamental architecture of these platforms will benefit you as a full-stack web developer.

Your task is to build the back end for an e-commerce site by modifying starter code. You’ll configure a working Express.js API to use Sequelize to interact with a MySQL database.

Because this application won’t be deployed, you’ll also need to provide a link to a walkthrough video that demonstrates its functionality and all of the acceptance criteria being met. You’ll need to submit a link to the video and add it to the readme of your project.

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

## Credit

Andrew Ngo

[link to GitHub Profile](https://github.com/MiinoSil)

## License

[LICENSE](./LICENSE.txt)
## Mock-Up (NOT author's work, example of what completed api should look like)

The following animation shows the application's GET routes to return all categories, all products, and all tags being tested in Insomnia:

![In Insomnia, the user tests “GET tags,” “GET Categories,” and “GET All Products.”.](./Assets/13-orm-homework-demo-01.gif)

The following animation shows the application's GET routes to return a single category, a single product, and a single tag being tested in Insomnia:

![In Insomnia, the user tests “GET tag by id,” “GET Category by ID,” and “GET One Product.”](./Assets/13-orm-homework-demo-02.gif)

The following animation shows the application's POST, PUT, and DELETE routes for categories being tested in Insomnia:

![In Insomnia, the user tests “DELETE Category by ID,” “CREATE Category,” and “UPDATE Category.”](./Assets/13-orm-homework-demo-03.gif)

Your walkthrough video should also show the POST, PUT, and DELETE routes for products and tags being tested in Insomnia.






* The walkthrough video must demonstrate POST, PUT, and DELETE routes for categories, products, and tags being tested in Insomnia.

