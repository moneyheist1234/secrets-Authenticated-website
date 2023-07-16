# secrets-Authenticated-website
secrets-Authenticated-website  inspired by Angele YuWeb Development
This is a web application called Secrets that allows users to anonymously share their secrets. The app uses authentication to ensure that only registered users can access and submit secrets. The following features and technologies are implemented in the app:

# Features
User registration and login: Users can register an account and log in using their email and password. The registration and login forms are implemented using HTML forms and handled by the server using the Express framework.

 Google OAuth 2.0 authentication: Users can also sign in using their Google accounts. The app utilizes the passport-google-oauth20 package to implement the Google OAuth 2.0 authentication strategy.

User sessions: The app uses express-session to manage user sessions, allowing users to stay authenticated across different pages and requests.

Database integration: The app uses MongoDB as the database to store user information and secrets. The mongoose package is used to connect to the MongoDB database and define the user schema.

Password hashing: User passwords are securely hashed and stored in the database using the passport-local-mongoose package. This package provides username/password authentication and simplifies the process of working with passwords in the app.

Access control: The app includes middleware functions to check if a user is authenticated before granting access to certain routes. The ensureAuthenticated middleware ensures that only authenticated users can access specific routes, such as submitting a secret.

Secrets submission: Authenticated users can submit their secrets through a form implemented using an HTML form and handled by an Express route. The submitted secrets are associated with the user and stored in the database.

# Authentication Used
Local authentication: Users can register an account and log in using their email and password. The passport-local-mongoose package is used to handle local authentication.

Google OAuth 2.0 authentication: Users can sign in using their Google accounts. The passport-google-oauth20 package is used to implement the Google OAuth 2.0 authentication strategy.

# Prerequisites
To run the Secrets app locally, make sure you have the following installed:

Node.js
npm (Node package manager)
MongoDB
# Installation

Clone the repository:

"git clone https://github.com/your-username/secrets-app.git"

# Install the dependencies:

cd secrets-app
npm install
Set up environment variables:

Create a .env file in the root directory.

Add the following variables to the .env file:

makefile
Copy code
CLIENT_ID=<your-google-client-id>
CLIENT_SECRET=<your-google-client-secret>
Replace <your-google-client-id> and <your-google-client-secret> with your own Google OAuth 2.0 credentials. You can obtain these credentials by creating a new project in the Google Cloud Console and enabling the Google OAuth 2.0 API.

# Start the application:


npm start
Open your web browser and visit http://localhost:3000 to access the Secrets app.
That's it! You can now register, log in, and start sharing your secrets anonymously.

Note: Make sure MongoDB is running on your local machine or update the url variable in server.js to point to your MongoDB server.

# contact
email: "praneeth.naik2002@gmail.com"



