# HTML Forms 

- this used to collect user input

```
<form>
    <input type="text"> ---/ display text input fiel
    <input type="radio"> ---/ display cercular buttons for selection
    <input type="checkbox"> ---/ checkbox
    <input type="submit"> ---/submit button
    <input type="button"> ---/ clicable button
</form>
```

- we can add name attribute to the input tag ,from that name we can add label for that input 

```
for examble 
<input type="checkbox" name=check1>
<label for=check1>checkbox1</label>

```

it will result 
- [ ] (checkbox1)

# CSS forms 
 
 to select items from a form you should folow the foloing method

 ```
 input [type=""]{

 }
 ```

 # CSS lists 

 we can change how list bullet point looks by 

 ```

 list-style-type : cicle
                        sequare
                        upper-roman
                        lower-roman
                        Upper-alpha
                        lower-alpha

list-style-img : url(imglink)

 ```

# CSS tables 

we can show the empty cells by 

```
empty-cells : show
```

we can controll how the cell if far from each other by 

```
border-spacing : 10px 10px --> seperate cells 

border-collapse : collapse --> no space between cells 
```


# JS event 

we can sensor event by using `document.addEventListener` and we can after sensoring run a fuction 

```
element = document.getElementById()
element.addEventListener("event (eg: on click)",function)

```




