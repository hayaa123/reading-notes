# react life cycle 

## Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

the render happens first in the render phase then the componentDidMount in the commit phase

## What is the very first thing to happen in the lifecycle of React?

Mounting --> creating component and inserting it to a dom

## Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

constructor --> render --> react update --> componentDidMount    --(if uncommit)--> componentWillUnmount

## What does componentDidMount do?

load anything using network request or initialize the do 

## Things I want to know more about

how to use react in more dynamic and flexable way and how to make a fuly functional website out of this library 

# React State Vs Props

-What types of things can you pass in the props?

any data type 

-What is the big difference between props and state?

state is internal and controlled by the component itself while props are external and controlled by whatever renders the component.
-When do we re-render our application?




resourses 

[this](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093) blog

[this](https://stackoverflow.com/questions/27991366/what-is-the-difference-between-state-and-props-in-react#:~:text=The%20key%20difference%20between%20props,by%20whatever%20renders%20the%20component.) stackoverflow question 