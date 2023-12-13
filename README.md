# nodejs-express-sequelize-postgresql

# npm init --initalize the node project

# install package -- npm install express sequelize pg pg-hstore cors --save

# setup expresss web server --server.js
        -- import express and cors modules
         . Express is for building apis
         . Cors provides Express middleware to enable CORS with various options.

– create an Express app, then add body-parser (json, urlencoded) and cors middlewares using app.use() method.
# Notice that we set origin: http://localhost:8081.
– define a GET route which is simple for test.
– listen on port 8080 for incoming requests.

- node server.js


# Configure postgress database and sequalize 
    In the app folder, we create a separate config folder for configuration with db.config.js


    First five parameters are for PostgreSQL connection.
    pool is optional, it will be used for Sequelize connection pool configuration:

    max: maximum number of connection in pool
    min: minimum number of connection in pool
    idle: maximum time, in milliseconds, that a connection can be idle before being released
    acquire: maximum time, in milliseconds, that pool will try to get connection before throwing error

    For more details, visit API Reference for the Sequelize constructor.

# Initialize Sequelize

    initialize Sequelize in app/models folder that will contain model in the next step.
    create models

# Create the Controller
Inside app/controllers folder, let’s create tutorial.controller.js with these CRUD functions:

# Define Routes
When a client sends request for an endpoint using HTTP request (GET, POST, PUT, DELETE), we need to determine how the server will reponse by setting up the routes

We also need to include routes in server.js (right before app.listen()):