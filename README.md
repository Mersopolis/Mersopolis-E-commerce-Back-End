# Mersopolis E-commerce Back End

## Badges
![MIT License](https://img.shields.io/badge/license-MIT%20License-green)

## Description
A Command Line Program to Manage the Back End for an E-commerce Organization

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Tests](#tests)
- [Questions](#questions)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

## Installation
1. Ensure you have Node.js installed. https://nodejs.org/en/ <br/>2. Ensure you have npm installed. https://docs.npmjs.com/downloading-and-installing-node-js-and-npm#using-a-node-installer-to-install-nodejs-and-npm <br/>3. Ensure you have a MySQL account. https://www.mysql.com/ <br/>4. Download the zip from GitHub under the Code dropdown menu. https://github.com/Mersopolis/Mersopolis-E-commerce-Back-End <br/>5. Extract the contents to a folder.

## Usage
Before using the program for the first time:<br/>1. Create a new file in the installation folder called<br/>.env<br/><br/>2. Enter these lines in the file:<br/>DB_NAME='ecommerce_db'<br/>DB_USER='root'<br/>
DB_PASSWORD='(Enter your MySQL password here)'<br/>3. Open your system's command line and ensure the current directory is the installation folder. (On Windows, you can hold Shift and right click while in the folder and select the "Open Command Window Here" or "Open PowerShell Window Here" option.)<br/>4. Run this command:<br/>npm install<br/><br/>5. Run this command:<br/>mysql -u root -p<br/><br/>6. Enter your MySQL password.<br/>7. Run this command:<br/>SOURCE db/schema.sql<br/><br/>8. Run this command:<br/>quit<br/><br/>Once dependencies are installed and database is initialized:<br/>1. Open your system's command line and ensure the current directory is the installation folder.<br/>2. Run this command:<br/>npm start<br/><br/>3. Use GET requests to view things. GET requests can be sent to /api/categories, /api/categories/:id, /api/products, /api/products/:id, /api/tags, and /api/tags/:id<br/>4. Use POST requests to make new things. POST requests can be sent to /api/categories with a JSON body formatted like so:<br/>{<br/> "category_name": "namehere"<br/>}<br/><br/>POST to /api/products like so:<br/>{<br/>  "product_name": "namehere",<br/>"price": 200.00,<br/>"stock": 3,<br/>"tagIds": \[1,2,5]<br/>}<br/><br/>POST to /api/tags like so:<br/>{<br/>  "tag_name": "namehere"<br/>}<br/><br/>5. Use PUT requests to update existing things. PUT requests can be sent to /api/categories/:id with a JSON body formatted like so:<br/>{<br/>  "category_name": "newnamehere"<br/>}<br/> PUT in /api/products like so:<br/>{<br/>  "product_name": "newnamehere",<br/>"price": 150.50,<br/>"stock": 4,<br/>"tagIds": \[4,5,7]<br/>}<br/><br/>PUT in /api/tags like so:<br/>{<br/>  "tag_name": "newnamehere"<br/>}<br/><br/>5. Use DELETE requests to delete existing things. DELETE requests can be sent to /api/categories/:id, /api/products/:id, /api/tags/:id<br/>6. To exit the program, press CTRL+C

## Tests
<br/>1. Create a new file in the seeds folder called<br/>.env<br/><br/>2. Enter these lines in the file:<br/>DB_NAME='ecommerce_db'<br/>DB_USER='root'<br/>DB_PASSWORD='(Enter your MySQL password here)'<br/>3. While the program is not active, open your system's command line and ensure the current directory is the installation folder.<br/>4. Run this command:<br/>npm seed<br/><br/>5. Start the program.<br/>6. You can use a program like Insomnia to test the routes. For example, send GET requests to localhost:3001/api/categories , localhost:3001/api/products , or localhost:3001/api/tags

## Questions
Questions can be directed to this GitHub profile or this email.

GitHub: [Mersopolis](https://github.com/Mersopolis)

Email: [mersopolis@gmail.com](mailto:mersopolis@gmail.com)

## Contributing
N/A

## Credits
Starter code provided by the University of Utah.<br/>Code expanded by me, Devon Ethington.<br/>Node.js https://nodejs.org/en/ <br/>npm https://www.npmjs.com/ <br/><br/>MySQL2 https://www.npmjs.com/package/mysql2?activeTab=code <br/>express https://www.npmjs.com/package/express <br/>dotenv https://www.npmjs.com/package/dotenv <br/>

## License
MIT License

Copyright (c) 2023 Devon Ethington
      
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

