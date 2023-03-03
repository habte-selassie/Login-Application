# Login-Application
Simple Login System with Express and Session Management
This is a simple login system built with Node.js, Express, and EJS that demonstrates how to manage user sessions in an Express application.
The application allows users to log in with a hard-coded email and password and view a dashboard page if they are authenticated. 
If they are not authenticated, they are redirected to the root page.

Installation and Setup
To use this application, you need to have Node.js and NPM (Node Package Manager) installed on your machine. Once you have installed them, follow these steps:

Clone the repository using the command:

bash
Copy code
git clone https://github.com/your_username/login-application.git
Change into the project directory using the command:

The application should now be accessible at http://127.0.0.1:8000/

bash
Copy code
cd simple-login-system
Install the project dependencies using the command:

bash
Copy code
npm install
Start the application using the command:

bash
Copy code
npm start
This will start the application on port 8000. You can access the application in your web browser at http://localhost:8000.

Usage
The application has a simple login form on the root page ("/") that allows users to enter their email and password. If the email and password match the hardcoded values, the user is redirected to the dashboard page ("/dashboard"). If not, an error message is displayed.

The dashboard page displays a welcome message with the user's email address. If the user is not authenticated, they are redirected to the root page.

The application also has a logout button on the dashboard page that allows users to log out and end their session.

File Structure
The application has the following file structure:

java
Copy code
simple-login-system/
├── node_modules/
├── public/
│   ├── assets/
│   │   ├── css/
│   │   └── js/
│   └── index.html
├── router.js
├── views/
│   ├── base.ejs
│   ├── dashboard.ejs
│   └── error.ejs
├── .gitignore
├── app.js
├── package-lock.json
├── package.json
└── README.md
The main application logic is contained in the app.js file. The router.js file contains the routes for the application. The views directory contains the EJS templates used to render the HTML pages. The public directory contains the static assets (CSS and JS files) used in the application. The node_modules directory contains the dependencies for the project. The .gitignore file specifies which files and directories should be ignored by Git. The package.json and package-lock.json files contain information about the project and its dependencies. Finally, the README.md file contains the documentation for the project.

# Dependencies
The application depends on the following NPM packages:

express: A fast, unopinionated, minimalist web framework for Node.js
body-parser: A middleware for parsing incoming request bodies
express-session: A middleware for managing user sessions in Express
ejs: A simple templating engine for generating HTML markup
These dependencies are specified in the package.json file and are installed automatically when you run npm install.
