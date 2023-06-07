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
https://api.imgur.com/3/gallery/${section || 'hot'}/${sort || 'viral'}/${window || 'day'}/${page || 1}?showViral=${!!showViral}&mature=false&album_previews=false

## This project structure
app : bootstraped with create-react-app
server: simple server with Express.js
Getting Started
First of all! Register your app with Imgur. To make Imgur API calls, you will need a "Client_ID" for Authorization. You can get Client_ID by registering your app with Imgur HERE.

FYI: While registering you app with Imgur Authorization callback URL: in the form can be # (need not be a valid URL, for development).

Once registered keep safe the "Client_ID", we will need it in the next step

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
Jest: A JavaScript testing framework.
react-testing-library: A testing library for React applications.
TypeScript: A typed superset of JavaScript.
## Backend:

Express.js: A web application framework for Node.js.
Axios: A promise-based HTTP client for making API requests.
TypeScript: A typed superset of JavaScript.
