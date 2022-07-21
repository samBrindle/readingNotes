# Class 04 Reading
## Classes and Objects
* Objects: an encapuslation of variables and functions into a single entity. Objects get their variables and functrinos from classes
* Classes: Templates to create your own objects
  * To assign vaiables in a class you use `def __init__(self,var)`

### Example of a class:
`class MyClass:
      var = "blah"
      
      def function(self):
          print("This is a message inside the class`
 
## Python Testing with pytest: Fixtures and Coverage
* Fixtures: objects that contain data you want to share across tests or involve the network or filesystem
  * Define a fixutre by using the combination of the pytest.fixture decorator and a function definition
  * `def reverse_lines(f): <br/>
          return [one_line.rstrip()[::-1] + '\n'<br/>
                for one_line in f]`
               
* Coverage: `pytest --cov=mymul` will give you a coverage report with your pytest
