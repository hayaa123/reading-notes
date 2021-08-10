# Css Transforms

used to size, position, and change elements.

```
element {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```

# CSS Transition 

we can modify the timing when changing thing by sit a transition time 

```
.box {
  background: #2db34a;
  transition-property: background, border-radius;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
  border-radius: 50%;
}
```

what we can make from the transition property ? 

- Fade in
- Change color
-  Grow & Shrink
- Rotate elements --> we also use transformer here  :D 
- Square to circle
- 3D shadow  --> we use also transformer here 
- Swing --> we use also transformer here
- Inset border