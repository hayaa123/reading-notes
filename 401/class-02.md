# In Tests We Trust - TDD with Python
```
A convention widely used is the AAA structure: 

- Arrange, Act and Assert.

- Arrange: you need to organize the data needed to execute that piece of code (input);

- Act: here you will execute the code being tested (exercise the behaviour);

- Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

TDD cycle 

- Write a unit test and make it fail 

- Write the feature and make the test pass!

- Refactor the code
```
# If name equals main

if w run the program in the terminal it wil give the `__name__` a value of `"__main__"` so the code under 
if __name__ == "__main__" will exceute just in the run of this file in terminal 

the other blocks of code can be imported in other files 

# Recursion

The process in which a function calls itself directly or indirectly


How memory is allocated to different function calls in recursion? 
```
When any function is called from main(), the memory is allocated to it on the stack. 

we should be carfull in recursion function becase it may cause stack overflow and block the memory if called in the wrong way (eg : infinity)
```


resourses 

[In Tests We Trust - TDD with Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

[If name equals main](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

[Recursion](https://www.geeksforgeeks.org/recursion/)