# List Comprehensions

### what ?

>List comprehension is a powerful and concise method for creating lists in Python that becomes essential the more you work with lists, and lists of lists.

### why ? 

> to keep your code elegant and readable, it’s recommended that you use Python’s comprehension features.

### how ? 

Syntax 

> `my_new_list = [ expression for item in list ]`

### example  

make a list of sequare numbers in range 10

```python 
list1 = [i**2 for i in reange (10)]
```
extract number from a string 

```python 
string = "12-34"
list2 = [int(i) for i in string if i.isdigit()]
```


# Decorator 

1- decorators wrap a function, modifying its behavior.

2- eg :
 ```python
 def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

def say_whee():
    print("Whee!")

say_whee = my_decorator(say_whee)

>>> say_whee()
Something is happening before the function is called.
Whee!
Something is happening after the function is called.

```

3- Syntactic Sugar! --> you can use decorator using `@` sympol

eg :
```python
def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

@my_decorator
def say_whee():
    print("Whee!")
```

resorses 

[List Comprehensions](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)

[Primer on Decorators](https://realpython.com/primer-on-python-decorators/)