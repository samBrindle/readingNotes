# API's
## API Design Best Practices
* What does REST stand for?
  * Representational State Transfer, an architectural style for building distributed systems based on hypermedia.
* REST APIs are designed around a ____.
  * Resources, any kind of object, data, or service that can be accessed by the client
* What is an identifier of a resource? Give an example.
  * A URI that uniquely identifies that resource. 
  * EX: https://adventure-works.com/orders/1
* What are the most common HTTP verbs?
  * GET, POST, PUT, PATCH and DELETE
* What should the URIs be based on?
  * Nouns (the resource) and not verbs (the operations on the resource)
* Give an example of a good URI.
  * https://adventure-works.com/orders 
* What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
  * A chatty web API means that it sends a large number of small resources. This is usually a bda thing because it requires more requests.
* What status code does a successful GET request return?
  * 200 or 204 depending on the content
* What status code does an unsuccessful GET request return?
  * 404
* What status code does a successful POST request return?
  * 201 or 200 or 204 depending on the content
* What status code does a successful DELETE request return?
  * 204
