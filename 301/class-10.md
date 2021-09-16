# Call stack  and error messages

## Understanding the JavaScript Call Stack

### What is a ‘call’?

is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

### How many ‘calls’ can happen at once?

2

### What does LIFO mean?

last in first out

### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

```
function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();
```

### What causes a Stack Overflow?

calling the function in its selft which will keep calling it untel she exceed the stack

## JavaScript error messages

### What is a ‘refrence error’?

this means that there are variable are  not defined

### What is a ‘syntax error’?

his occurs when you have something that cannot be parsed in terms of syntax

### What is a ‘range error’?

Try to manipulate an object with some kind of length and give it an invalid length

### What is a ‘tyep error’?

this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible,

### What is a breakpoint?

selecting a point where you want to checkout with the depugger to focus on

### What does the word ‘debugger’ do in your code?

runs the code step by step and shows the output

### Things I want to know more about

the debugging skills 

### resorses

[Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

[JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)