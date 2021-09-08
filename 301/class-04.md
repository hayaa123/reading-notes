# React Docs - Forms

## What is a ‘Controlled Component’?

a compontnent that containes a state ,and when event occure the state of the component can be changed by setState()
.
## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

I think both of these option will work, but I prefer the first one  

## How do we target what the user is entering if we have an event handler on an input field?

extacting the value from the targeting event by writing `evnent.targrt.value `

# The Conditional (Ternary) Operator Explained

## Why would we use a ternary operator?

to make smaller lines of code and make it more readable 

## Rewrite the following statement using a ternary statement:

  ```
    if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
  ```
in ternary statment 

```
X===y ? console.log(true) : console.log(false)
```

## Things I want to know more about

how to handle multiple events in a controlled component 

resorses

[React Docs - Forms](https://reactjs.org/docs/forms.html)

[ternary operator](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)