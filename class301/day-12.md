# CRUD
## Status Codes Based on REST Methods
In your own words, describe what each group of status code represents:

100’s = Informational codes that refer to the Header part of a request
200’s = Success codes, letting the client know their request was accepted
300’s = Redirection codes, let the client know their resource isn't available
400’s = Client Error Codes, timeouts, wrong URI, missing authentication, ect
500’s = Servoer Error Codes, usually related to an overwhelmed server
* What is a status code 202?
  * Tells the client that the request was valid but its still processing something
* What is a status code 308?
  * A permanent Redirect
* What code would you use if an update didn’t return data to a client?
  * 204 No Content
* What code would you use if a resource used to exist but no longer does?
  * 410 Gone
* What is the ‘Forbidden’ status code?
  * 403 Forbidden

## Build A REST API with Node.js, Express, & MongoDB - QUICK  
* Why do we need to pull our MongoDB database string out of our server and put it into our .env?
  * So that not everyone can access it.
* What is middleware?
  * Software that acts as a bridge
* What does app.use(express.json()) do?
  * It parses incoming jSON requests and puts the parsed data in req
* What does the /:id mean in a route?
  * It is a param name
* What is the difference between PUT and PATCH?
  * PUT is a method modifying resource where the client sends data that updates the entire resource
  * PATCH is a method modifying resource where the client sends partial data that is updated without modifying the entire data
* What does a 500 error status code mean?
  * The server encountered an unexpected condition that precented it from fulfilling the request
* What is the difference between a status 200 and a status 201?
  *  200: The request was recieved and understood and is being processed
  *  201: The request was successful and as a result, a resource has been created
