# Pythonisms

- What Are Dunder Methods
    - special methods are a set of predefined methods you can use to enrich your classes

- How do for-in loops work in Python?
At this point we’ve got our Repeater class that apparently supports the iterator protocol, and we just ran a for-in loop to prove it:
```
repeater = Repeater('Hello')
for item in repeater:
    print(item)
```
