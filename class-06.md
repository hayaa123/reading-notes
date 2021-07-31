# JS objects 

each object contains properties and these properties contains values 
object are variables but can contain many values 

How to do it ? 

```
const object_name = {property_name:value ,property_name:value etc.}
```

we can access object properties by wrrite :

```
object_name.property_name --> outputs value

we call this (.property_name) by method 

```
also we can write 

```
object_name[property_name]
```
# Document Object Model (DOM)

+ it is constructed as tree model 
 
 ![tree DOM](https://www.w3schools.com/js/pic_htmltree.gif)

 + the Html DOM ----> get and change HTML elements but how ? :D 

 first we should know  what is method and property ,the mehod are the actions can done while property are values that you can 
 change or set . 
 there are some method we can use to get the html element like :

 ```
 document.getElementById(id) --> as its name idicated it find an element by passing its Id inside the parentheses after it 
 document.getElementsByTagName(name)
 document.getElementsByClassName(name)	
 ```

 now we know how to get element what about changing it :D 

after getting element we can change it from the properties in DOM as 

```
document.getElementById(id).innerHTML = "" --> change HTML content 
document.getElementById(id).attribute = "" --> change the attribute value 

```
