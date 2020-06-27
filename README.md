# Web-API
Using Mongo DB’s sample “Sales” data and leveraging NodeJS, Express, pushed a Web Service with API endpoints to Heroku which responds to http requests

# End-point

https://rocky-caverns-39016.herokuapp.com/api/sales/

# Routes

## POST /api/sales
This route uses the body of the request to add a new "Sale" document to the collection and return a success / fail message to the client.

## GET /api/sales
This route must accept the numeric query parameters "page" and "perPage", ie: /api/sales?page=1&perPage=5. It will use these values to return all "Sales" objects for a specific "page" to the client.

## GET /api/sales
This route must accept a numeric route parameter that represents the _id of the desired sale object, ie: /api/sales/5bd761dcae323e45a93ccfe8. It will use this parameter to return a specific "Sale" object to the client.

## PUT /api/sales
This route must accept a numeric route parameter that represents the _id of the desired sale object, ie: /api/sales/5bd761dcae323e45a93ccfe8 as well as read the contents of the request body. It will use these values to update a specific "Sale" document in the collection and return a success / fail message to the client.

## DELETE /api/sales
This route must accept a numeric route parameter that represents the _id of the desired sale object, ie: /api/sales/5bd761dcae323e45a93ccfe8. It will use this value to delete a specific "Sale" document from the collection and return a success / fail message to the client.
