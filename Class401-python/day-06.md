# Reading 06 - Ten Thousand Game 1

## How to use Random Module
* When to use it?
  * Picking a random element from a list
  * Picking a random card from a deck
  * Flipping a coin
  * Making your password database more secure
* Random Functions
  * Randint
    * Provides a random integer from two parameters
    * `import random`


       `print random.randint(0,5)`
       
    * Will output either 1, 2, 3, 4, or 5
  * Random
    * Provides a random number from [0.0, 1.0)
    * Multiply by a number if you want a larger number
    * `random.random() * 100`
    * would return a number between 0, 100
  * Choice
    * Generate a random value from the sequence sequence
    * random.choice( ['red', 'black', 'green'] )
    * will return either red, black, or green
  * Shuffle
    * Shuffles elements in a list so they are in a random order
  * Randrange
    * Generates a randomly selected element from range(start, stop, step)

## What is Risk Analysis
* Risk analysis is th eprocess of identifying the risks in applications or software that you built and prioritizing them to test
* Another part is the categorization of risks and the impact of the risk
* Why use Risk Analysis
  * To highlight potential problem areas
  * Helps developers and managers mitigate risks
* Possible risks:
  * Use of new hardware
  * Use of new technology
  * Use of new automation tool
  * The sequence of code
  * Availabilty of test resources for the application
* Unavoidable Risks:
  * Time you allocated for testing
  * Defect leakage due to the complexity or size of the application
  * Urgency from the clients to deliver the project
  * Incomplete requirements
* Steps to tackle these issues:
  * Conduct Risk Assessment review meeting
  * Use maximum resources to work on high-risk areas
  * Create a Risk Assessment database for future use
  * Identify and notice the risk magnitude indicators:
    *  High - the effect of the risk would be very high and non-tolerable. The company might face loss
    *  Medium - tolerable but not desirable. The company may suffer financially but there is a limited risk
    *  Low - tolerable. There lies little or no external exposure or financial loss
* Risk Identification
  * Business Risks: Most common. Risk that may come from your company or customer, not the project
  * Testing Risks: Be well aquainted with the platform you are working on and the software testing tools being used
  * Premature Release Risk: Fair amount of knowledy to anakyze the risk associate with releasing unsatisfactory or untested software
  * Software Risks: Be well versed with the risks associated with the software development process
* Risk Assessment
  * Effect: To assess risk by Effect. In case you identify a condition, event, or action and try to determine its impact
  * Cause: To assess risk by Cause is opposite of by Effect. Initialize scanning the problem and reach to the point that could be the most probable reason behind that
  * Likelihood: To assess risk by Likelihood is to say that there is a probabilty that a requirement won't be satisfied
