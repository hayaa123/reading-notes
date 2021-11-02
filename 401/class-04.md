# Classes and Objects

> Classes are essentially a template to create your objects.

class in code 

```
class ClassName:       # this is foe define the class
    def __init__ (self,x,y):    # this functiomget called when inisializing the class
        self.x = x    # self refer to the class 
        self.y =y 
    
    def print_self(self):
        print(self.x + self.y )   # note that we put self here also to call this class properties 

```

# Thinking Recursively

- Recursion means calling the function in its self it contain a base case and general case 

- it can be used to make sequences

- to solve recursion propblems we should :
 >   1)Decompose the original problem into simpler instances of the same problem

 >  2)As the large problem is broken down into successively less complex ones, those subproblems must eventually become so simple that they can be solved without further subdivision. This is the base case



# Pytest Fixtures and Coverage

> - to run function in pytest the function name should start with test

> -  rather than defining global variables in your test file, you can create a fixture that'll provide your test with the appropriate object at the right time. --> @pytest.fixture 

[Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)
[Thinking Recursively](https://realpython.com/python-thinking-recursively/)
[Pytest Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)