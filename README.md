## Image gallery (Imgur gallery API)
This is a web application that allows browsing the Imgur gallery using the Imgur API. It displays gallery images in a grid of thumbnails and provides various filtering options. When clicking on an image, it shows detailed information about the image.

## Features
Browse the Imgur gallery.
Filter the gallery by section: hot, top, user.
Include or exclude viral images from the result set.
Specify window and sort parameters.
Click on an image to view its details.
Pagination for browsing multiple pages of the gallery.

## API: official
https://api.imgur.com/3/gallery/{{section}}/{{sort}}/{{window}}/{{page}}?showViral={{showViral}}

## This project structure
app : bootstraped with create-react-app
server: simple server with Express.js
Getting Started
First of all! Register your app with Imgur. To make Imgur API calls, you will need a "Client_ID" for Authorization. You can get Client_ID by registering your app with Imgur HERE.

FYI: While registering you app with Imgur Authorization callback URL: in the form can be # (need not be a valid URL, for development).

Once registered keep safe the "Client_ID", we will need it in the next step

## Prerequisites
Node.js (version v18.10.0)
npm (version 9.6.7)
Installation
Clone the repository: git clone https://github.com/EgresaMeto/imgur-fullstack.git

Navigate to the client directory: cd imgur-redux

Install the client dependencies: npm install

Navigate to the server directory: cd ../server

Install the server dependencies: npm install

Development
Start the client-side React app: cd imgur-redux npm start
The React app will be running on http://localhost:3000.

Start the server-side Node.js app: cd ../server npm start
The server will be running on http://localhost:9000.

Production Build
To create a production-ready build of the client-side React app, run the following command from the client directory: npm run build

## Setting up server
cd server
create file nodemon.json and the following line
{"env":{"client_id": "<Client_ID>"}}
Where <Client_ID> is the one you got from registering your app with Imgur above
npm install
npm start

## Setting up app
cd app
npm install
npm start


## Technologies Used
## Frontend:

React: A JavaScript library for building user interfaces.
Redux: A predictable state container for managing application state.
Styled Components: A CSS-in-JS library for styling components.
TypeScript: A typed superset of JavaScript.
## Backend:

Express.js: A web application framework for Node.js.
Axios: A promise-based HTTP client for making API requests.
TypeScript: A typed superset of JavaScript.
