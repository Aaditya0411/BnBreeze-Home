name: BnBreeze
type: Full Stack Web Application
inspired_by: Airbnb

description: >
  BnBreeze is a full-stack Airbnb-style web application.
  It allows users to create, view, edit, and delete property listings,
  upload images, add reviews, and view locations using maps.
  The project follows MVC architecture with secure authentication.

features:
  authentication:
    - User signup and login
    - Session based authentication
    - Authorization using middleware
  listings:
    - Create listing
    - Edit listing
    - Delete listing
    - View all listings
  reviews:
    - Add review
    - Delete review
  media_and_location:
    - Image upload using Cloudinary
    - Geocoding using MapTiler
  ui:
    - Fully responsive UI
    - Flash messages for success and error
    - Custom 404 error page with Explore option

tech_stack:
  frontend:
    - HTML
    - CSS
    - JavaScript
    - EJS
  backend:
    - Node.js
    - Express.js
  database:
    - MongoDB Atlas
    - Mongoose
  authentication:
    - Passport.js
    - Passport-Local-Mongoose
  middleware:
    - Express-Session
    - Connect-Flash
    - Multer
    - Joi
  cloud:
    - Cloudinary
    - MapTiler

project_structure:
  controllers:
    - listings.js
    - reviews.js
    - users.js
  models:
    - listing.js
    - review.js
    - user.js
  routes:
    - listing.js
    - review.js
    - user.js
  views:
    layouts:
      - boilerplate.ejs
    includes:
      - navbar.ejs
      - footer.ejs
      - flash.ejs
    listings:
      - index.ejs
      - show.ejs
      - new.ejs
      - edit.ejs
    users:
      - login.ejs
      - signup.ejs
    error:
      - error.ejs
  public:
    css:
      - style.css
      - rating.css
    js:
      - script.js
  utils:
    - ExpressError.js
    - wrapAsync.js
  root:
    - app.js
    - cloudConfig.js
    - schema.js
    - package.json
    - README.md

how_to_run:
  prerequisites:
    - Node.js installed
    - MongoDB Atlas account
    - Cloudinary account
    - MapTiler API key
  steps:
    - git clone https://github.com/Aaditya0411/BnBreeze-Home.git
    - cd BnBreeze-Home
    - npm install
    - create .env file
    - add environment variables
    - node app.js
  default_port: 3000

environment_variables:
  MONGO_URI: MongoDB connection string
  CLOUDINARY_CLOUD_NAME: Cloudinary cloud name
  CLOUDINARY_API_KEY: Cloudinary API key
  CLOUDINARY_API_SECRET: Cloudinary API secret
  MAPTILER_API_KEY: MapTiler API key

learning_outcomes:
  - MVC architecture
  - Authentication and authorization
  - RESTful routing
  - Image upload handling
  - Cloud integration
  - Error handling and validation

author:
  name: Aaditya Goswami
  role: B.Tech CSE Student
  github: https://github.com/Aaditya0411
