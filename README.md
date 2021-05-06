# E-Commerce_Back_End

## Description

A functional Express.js API mock-up for an internet retail company database. Using the MySQL database created (ecommerce.db), you have access to create products, categories, and tags for the products.   

![badge](https://img.shields.io/badge/license-MITLicense-brightorange)

You can access more badges and their purposes at [shields.io](https://shields.io)

## Table of Contents
  * [Installation](#installation)
  * [Usage](#usage)
  * [Testing](#testing)
  * [Questions](#questions)
  * [License](#license)
    
    
## Installation
    
  _Follow these steps to properly install this application:_

  Once you have cloned the repository, npm install will set up the dependencies, `Express.JS`, `MySQL2`, `dotenv`, and `Sequelize`. `Nodemon` is also available to watch for changes and instantly refresh your browser. You will also need to have `MySQL` installed locally to create the server for the application. 
      
## Usage

  <p>&nbsp</p>

  ### Table_Of_Contents
  * [Install MySQL](#Install_MySQL)
  * [Create The Database](#Create_Database)
  * [Seed The Database](#Data)
  * [Start Server](#Start_Server)
  * [Adding & Deleting Data](#Add_Delete)
  * [Full Video Walkthrough](#Walkthrough)

  <p>&nbsp</p>

  _Instructions for use:_

  <p>&nbsp</p>

  ### Install_MySQL

  <p>&nbsp</p>

  This application requires you to have `MySQL` installed on your local computer. You can find more information about how to download, documentation, and the different services they offer at their website [https://www.mysql.com/](https://www.mysql.com/). 

  <p>&nbsp</p>

  ### Create_Database

  <p>&nbsp</p>

  Once `MySQL` is installed on your local computer, you simply clone this repository into your local computer, and in the root folder `e-commerce` type into your command line interface, `npm install`. This will run your node package manager and give your dependencies the files they need. We need to connect our server and create the database that will hold your data. The video below demonstrates this. Running `mysql -u root -p` will instantiate MySQL. This creates a User of `root` and you will be prompted to enter the password you created for your MySQL server. Then enter `source db/schema.sql`, this will create the database `ecommerce_db` from the schema.sql file. Once this is done, simply type `exit`.

  Also, the password and username for your MySQL should be placed in a file in the root of the project called `.env` this is a `.gitignore` file so it will not be publicly displayed. Use the following template: `DB_NAME='YourDatabaseNameHere'`,`DB_USER='root'`,`DB_PW='YourPasswordHere'`. The `dotenv` will place those variables in your `connection.js` file without public display automatically.

  <p>&nbsp</p>

  ![gif video showing mysql instatiated from CLI](assets/images/e-commerce_walkthrough_1.gif)

  <p>&nbsp</p>

  ### Data

  <p>&nbsp</p>

  For convenience, there is data provided to test the application and any changes you may want to make. This is activated by entering `npm run seed` this takes the seed data from the seeds folder and populates the corresponding data tables. This is shown in the example video below.

  <p>&nbsp</p>

  ![gif showing CLI seeding database](assets/images/e-commerce_walkthrough_2.gif)

  <p>&nbsp</p>

  ### Start_Server

  [Back to top](#E-Commerce_Back_End)

  <p>&nbsp</p>

  After the database has been seeded with mock data we can start our server running `npm start` in the CLI and we can see our first `GET` request to categories is succesful! We can access both the `Product` table and the `Tag` table in the same way. We can also get individual data by id number as well.

  _For all functionality watch the full length video at the bottom of the [Usage](#Walkthrough) section._

  <p>&nbsp</p>

  ![gif showing CLI starting server and Insomnia testing get request](assets/images/e-commerce_walkthrough_3.gif)

  <p>&nbsp</p>

  ### Add_Delete

  <p>&nbsp</p>

  We can add, delete, and edit table data as well. These functions are available in all three tables. The video demonstration below shows us implementing the `POST` function in Insomnia, which will add a new row to the `Category` table.

  <p>&nbsp</p>

  ![gif showing app testing in Insomnia](assets/images/e-commerce_walkthrough_4.gif)

  <p>&nbsp</p>

  Another example below shows us editing a `Category` table row from the `category_name` of `Belts` to `Sombrero`. We can then see by using the `GET` request by id number the change is saved in our table.

  <p>&nbsp</p>

  ![gif showing edit function testing in Insomnia](assets/images/e-commerce_walkthrough_5.gif)

  <p>&nbsp</p>

  The following GIF shows the `DELETE` in action. We take a category we created, delete by the id number, and when we search for the same id number, we now see it has been deleted from the database.

  <p>&nbsp</p>

  ![gif showing delete function testing in Insomnia](assets/images/e-commerce_walkthrough_6.gif)

  <p>&nbsp</p>

  [Back to top](#E-Commerce_Back_End)

  <p>&nbsp</p>

  ### Walkthrough
  
  [Full-length Video Walkthrough.](https://www.awesomescreenshot.com/video/3651954?key=6a7eb236d9d25767694e14247fcba405)

<p>&nbsp</p>

## Thank You & Contributions

<p>&nbsp</p>

**Thank you for your time.**

_Oringinal [code](https://github.com/coding-boot-camp/fantastic-umbrella.git) structure by Xander Rapstine._ His page is here at his GitHub: [Xandromus](https://github.com/Xandromus)

<p>&nbsp</p>

## Testing

  _Instructions for testing application:_

  Testing this application is best done through [Insomnia](https://insomnia.rest/), as you can review the [Usage](#Usage) instructions video demonstration of this while you test on your local computer. You could also use `MySQLWorkbench`, a developer download is here [https://dev.mysql.com/downloads/workbench/](https://dev.mysql.com/downloads/workbench/). Also more information and documentation here [https://www.mysql.com/products/workbench/](https://www.mysql.com/products/workbench/). However this is not demonstrated. Feel free to reach out with any questions about either application.
      
## Questions
      
  _For further questions:_

  Feel free to reach out on GitHub or email me.
  
  _Contact Info:_

  GitHub: [JOHNBANAS](https://github.com/JOHNBANAS)

  Email: [jbanas9124@gmail.com](mailto:jbanas9124@gmail.com)
    
## License

      
  _This application has the MIT License._
      
  For more information please view the [license description](https://choosealicense.com/licenses/mit/).
  
  