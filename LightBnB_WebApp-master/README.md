# LightBnB

## Project Structure

```
├── public
│   ├── index.html
│   ├── javascript
│   │   ├── components 
│   │   │   ├── header.js
│   │   │   ├── login_form.js
│   │   │   ├── new_property_form.js
│   │   │   ├── property_listing.js
│   │   │   ├── property_listings.js
│   │   │   ├── search_form.js
│   │   │   └── signup_form.js
│   │   ├── index.js
│   │   ├── libraries
│   │   ├── network.js
│   │   └── views_manager.js
│   └── styles
├── sass
└── server
  ├── apiRoutes.js
  ├── database.js
  ├── json
  ├── server.js
  └── userRoutes.js
```

* `public` contains all of the HTML, CSS, and client side JavaScript. 
  * `index.html` is the entry point to the application. It's the only html page because this is a single page application.
  * `javascript` contains all of the client side javascript files.
    * `index.js` starts up the application by rendering the listings.
    * `network.js` manages all ajax requests to the server.
    * `views_manager.js` manages which components appear on screen.
    * `components` contains all of the individual html components. They are all created using jQuery.
* `sass` contains all of the sass files. 
* `server` contains all of the server side and database code.
  * `server.js` is the entry point to the application. This connects the routes to the database.
  * `apiRoutes.js` and `userRoutes.js` are responsible for any HTTP requests to `/users/something` or `/api/something`. 
  * `json` is a directory that contains a bunch of dummy data in `.json` files.
  * `database.js` is responsible for all queries to the database. 
  
  ![Main page when logged in](/LightBnB_WebApp-master/assets/Main-page.png)
  ![Create a new listing](/LightBnB_WebApp-master/assets/new%20-property.png)

  ## Getting started
* Create a new repository using this repository as a template.
* Clone your repository onto your local device.
* Change directory into LightBnB_WebApp-master
* Install dependencies using the npm install command.
* Start the web server using the npm run local command. The app will be served at http://localhost:3000/.
* Go to http://localhost:3000/ in your browser.

## Dependancies 
* bcrypt 3.0.6
* body-parser 1.19.0
* cookie-session 1.3.3
* dotenv 16.0.3
* express 4.17.1
* nodemon 1.19.1
* pg 8.8.0