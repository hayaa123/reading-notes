# CSS 
Css is cascading style sheets made to make your HTML looks prettier

- syntax : it has a simple syntax you just have to specifie the elemrent you want to change and then start styling it :D 
```
element {
  styling 
}
```

- add it to html : actually there is 3 ways to write css in the html file
```
inline method --> put your style in the tag 
<h1 style = "property : value "></h1>

write it in the head 
<head>
<style>
element {
  properte : value 
}
</style>
</head>

and the most convienent was is the external method (to write a separate css file then link it in HTML file )
<head>
<link href="style.css">
</head>
```
lets discuss about the color property :

color can be represented in multiple ways 

1- using hex value --> 
> body {color: #92a8d1;}
2- using RGB  value --> 
> body {color: rgb(201, 76, 76);}

3- using heRGBA  value --> 
> body {color: rgba(201, 76, 76, 0.6);}

4- using HSL value --> 
> body {color: hsl(89, 43%, 51%);}


5- using HSLA value --> 
> body {color: hsla(89, 43%, 51%, 0.6);}

