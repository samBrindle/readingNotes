# Reading - Authentication and Production Server
## JSON Web Tokens
* JWT - a compact, self-contained way for securely transmitting information between parties as a JSON object

### When should you use JSON Web Tokens
* Authorization
* Information Exchange

### What is the JSON Web Token structure
Compact form consists of:
* Header
  * consists of two parts: token type and signing algorithm
* Payload
  * Contains the claims
  * Three types of claims: registered, public, and private
* Signature
  * encoded header
  * encoded payload
  * secret
  * algorithm
* `xxxxx.yyyyy.zzzzz`

## How to use JWT Authentication with Django REST Framework
* Install django's JWT library
* `pip install djangorestframework_simplejwt`
* add it to REST_FRAMEWORK in settings.py
* add new paths in the urls.py
