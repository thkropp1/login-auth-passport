# Complete Guide to Node Authentication with MySQL


Current version database is ported to MySQL

We will be using Passport to authenticate users locally 

## Instructions

login-auth-passport information:

To run the app(uses port 8080):

1. From top directory in git bash, type:
   npm install
2. cd to config folder and open database.js and also config.json, and change the mySQL connection 
   information to your credentials.
3. Go back to top directory in git bash and cd to scripts folder and type:
   node create_database 
4. Go back to top directory in git bash and type:
   node server
5. Go to browser and type:
   http://localhost:8080

------------------------------------------------------------------------------------
Folders:

config: database.js, config.json - Setup your mySQL connection login information
                      

scripts: create_database.js - Calls database.js and creates the database and the 
                              users table


package.json's dependencies:

"bcrypt-nodejs": "0.0.3",
"body-parser": "^1.15.2",
"express": "^4.14.0",
"express-session": "^1.14.2",
"mysql2": "^1.3.6",
"passport": "^0.3.2",
"passport-local": "^1.0.0",
"sequelize": "^4.3.1"
