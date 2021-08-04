# Java script Erorrs 
 
java script have multiplt error objects aas :

- SyntaxError --> error in writing the syntax of the code 
- ReferanceError --> when try to referance to non exist variable 
- TypeError --> when the value is not in expected data type 
- RangeError --> number is not in an acceptable range 
- URIError --> URI methods working incorrectly 
- EvalError --> eval() function not used correctly 

# handiling exceptions 

- `try` --> will ler you to test a block of code for error 

- `catch` --> lets you handle the error 

```
try {
    a block of code to try
}
catch(err){
    block of code to handle errors     --> err is the error message resulted from try we can prompt it or add it to the html 
}

```

- `throw` --> lets you create custom error 
 
```
try {
    if (codition) throw "error message"   
}
catch (err){
    block of code to handle errors -->when using the err here it will return the error message we write in throw 
}
```
heres a [W3 example](https://www.w3schools.com/js/tryit.asp?filename=tryjs_throw_error) makes you understand this better 

- `finaly` --> lets you execute code 


```
try {
    block of code
}
catch(err){
    error handiling 
}
finally {
    block of code executed regardless of try / catch result
}
```
> qouted from W3School
