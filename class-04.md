# HTML links 

we can make links in html using ancoanchor tag `<a>`
this tag has the attributes :
+ `href= ""` -- > here we put the link URL 
+ `target =""` --> use it to determine where to open the link 
   the values to enter in target are :
   `_self` --> opens in the same tap 
   `_parent` --> open in a perant tap 
   `_blank` -->
   `_top` --> open in the whole window

note : you can put image or tect inside the link so when chlick on it the link will open 


# CSS layout 

layout is very usefull in managing the web design and divide it into parts
we can devide our website to 3 main section and divide them as we want 
the main sections are `<header>` , <`main`> and `<footer>`

note : some element can call box element (taking the hole line it is on) and other called inline element takes just as it fit 

what we can do with layout ? 
+ positioning property --> we can but the following values in it `static` ,`relative`,`fixed` ,`absolute` and `sticky` 
+ floating --> `right` --> will put the box we selecte at the write and the other component continues on the left
+ clear --> specifiy what should happen to the element next to the floating element its values are `right`,`left `,`both`,`none` and `inherit`

# javascript functions 

why do we use functions ? 
1) its make youe code more readable 
2) avoid repititve work 
3) can use more than one time 

how do we use functions ?
```
function its_name (parameters){
    block of code
}
```
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

