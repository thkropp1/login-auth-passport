# Complete Guide to Node Authentication with MySQL


Current version database is ported to MySQL

We will be using Passport to authenticate users locally 

## Instructions

If you would like to download the code and try it for yourself:

1. Clone the repo: `git clone git@github.com:thkropp1/login-auth-passport.git`
1. Install packages: `npm install`
1. Edit the database configuration: `config/database.js`
1. Create the database schema: `node scripts/create_database.js`
1. Launch: `node server.js`
1. Visit in your browser at: `http://localhost:8080`

Folders:

app: routes.js 

config: database.js - Setup your mySQL connection login information

        passport.js - Login and signup authentication. Inserts new user's 
                      information into users table.
                      Line 64 is hardcoded with a dummy displayname(first and last 
                      name) - need to write the code to grab the first and last name 
                      input from the signup page.

scripts: create_database.js - Calls database.js and creates the database and the 
                              users table

views: index.ejs - main page to either login or signup new user

       login.ejs - login page

       profile.ejs - displays the user's profile information from the users table.
                     This is where you would put the flashcard pages instead.

       signup.ejs - signup page for new users

File:

package.json's dependencies:

"bcrypt-nodejs": "0.0.3",
"body-parser": "^1.13.1",
"connect-flash": "^0.1.1",
"cookie-parser": "^1.3.5",
"ejs": "^2.3.2",
"express": "^4.13.0",
"express-session": "^1.11.3",
"morgan": "^1.6.0",
"mysql": "^2.7.0",
"passport": "^0.2.2",
"passport-local": "^1.0.0"


