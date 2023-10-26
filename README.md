# RESTfulAPI_Test
Flask REST API for a drinks database

This is a simple Flask REST API for a drinks database. It allows you to perform the following CRUD operations:

Get all drinks:GET /drinks
Get a single drink by ID:GET /drinks/<id>
Add a new drink:POST /drinks
Update a drink:PUT /drinks/<id>
Delete a drink:DELETE /drinks/<id>
To use the API, you can send HTTP requests to the following endpoints:

GET /drinks
GET /drinks/<id>
POST /drinks
PUT /drinks/<id>
DELETE /drinks/<id>
The responses from the API will be in JSON format.

Here are some examples of how to use the API:

# Get all drinks
curl http://localhost:5000/drinks

# Get a single drink by ID
curl http://localhost:5000/drinks/1

# Add a new drink
curl -X POST http://localhost:5000/drinks \
  -H "Content-Type: application/json" \
  -d '{
    "name": "Margarita",
    "description": "A classic tequila cocktail with lime and orange liqueur."
  }'

# Update a drink
curl -X PUT http://localhost:5000/drinks/1 \
  -H "Content-Type: application/json" \
  -d '{
    "name": "Spicy Margarita",
    "description": "A margarita with a kick of jalapeño."
  }'

# Delete a drink
curl -X DELETE http://localhost:5000/drinks/1
You can also use the API with a Postman client or another HTTP client.

To run the API:

flask run
This will start the API on port 5000. You can then access the API at http://localhost:5000.

Dependencies:

Flask
Flask-SQLAlchemy
SQLAlchemy
Deployment:

You can deploy the API to a production server using a variety of methods, such as Heroku, AWS Elastic Beanstalk, or Docker.

Additional features:

Authentication and authorization
Pagination
Search
Versioning
Documentation
