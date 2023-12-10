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