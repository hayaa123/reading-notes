# React Docs - thinking in React

## How would you break a mock into a component heirarchy?

 breack them into boxes aand decide that using single responsibility principle, that is, a component should ideally only do one thing

## What is the single responsibility principle and how does it apply to components?

means that every component have one perpose 

## What does it mean to build a ‘static’ version of your application?

component reuse parent passing values using props 

## Once you have a static application, what do you need to add?

states and finctions then determine where srate will live and then add an inverse data flow

## What are the three questions you can ask to determine if something is state?

dose it changes overtime ? if unchanged then it isn’t state
is it passed from a parent as props ? if yes the it isn’t state
Can you compute it based on any other state or props in your component? If so, it isn’t state.

## How can you identify where state needs to live?

1) idntify components 

2) find a common owner component 

3)Either the common owner or another component higher up in the hierarchy should own the state.

4)Either the common owner or another component higher up in the hierarchy should own the state.

## Things I want to know more about

writing a clean,dynamic and readable code :D


### resorses


[React Docs - thinking in React](https://reactjs.org/docs/thinking-in-react.html)

[static-content](https://blog.stackpath.com/static-content/)
