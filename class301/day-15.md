# Authentication
## What is 0Auth
* What is OAuth?
  * An open-standard authorization protocol/framework
* Give an example of what using OAuth would look like.
  * Logging onto a website and it offers one or more opportunities to log on using another website's/service's logon
* How does OAuth work? What are the steps that it takes to authenticate the user?
  * Website_1 connects to the second website on behald of user
  * Webiste_2 generates a one-time token and a one-time secret unique to the transaction and parties involved
  * Website_1 gives this token and secret to the initiating user's client software
  * Client's software presents request token and secret to their authoraization provider
  * If not authenticated the client may be asked to authenticate. After, the client is asked to approve the authorization transaction to website_2
  * User approves a particular transaction type at website_1
  * User is given approved access token
  * User gives approved token to website_1
  * website_1 gives token to website_2 for proof of authentication
  * User sees successfully completed transaction
* What is OpenID?
  * Is for humans logging into machines while 0Auth is machines logging into machines

## Authorization and Authentication flows
* What is the difference between authorization and authentication?
  * Authentication: Determines whether users are who they claim to be
  * Authorization : Determines what users can and cannot access
* What is Authorization Code Flow?
  * Exchanging Authorization Code for tokens
* What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
  * Its Authorization Code Flow with additional security called Proof Key of Code Exchange
* What is Implicit Flow with Form Post?
  * An alternative to Authorization Code Flow intended for Public Clients
  * Provides Implicit Flow to securely store Client Secrets
* What is Client Credentials Flow?
  * Machine to machine applications running on your back-end, the system authenticates and authorizes the app rather than the user
* What is Device Authorization Flow?
  * Input-constrained devices that connect to the internet, the device asks the user to go to a link on their computer/smartphone and authorize it
* What is Resource Owner Password Flow?
  * Requests that users provide credentials typically using an interactive form
