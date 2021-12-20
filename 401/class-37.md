# React

- JSX -> syntax extension to JavaScript

- Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both.

- Elements are the smallest building blocks of React apps.

- React Only Updates What’s Necessary

- Handling Events 
    - React events are named using camelCase, rather than lowercase.
    - With JSX you pass a function as the event handler, rather than a string

    `onclick` `onsubmit`
```
unction tick() {
  const element = (
    <div>
      <h1>Hello, world!</h1>
      <h2>It is {new Date().toLocaleTimeString()}.</h2>
    </div>
  );
  ReactDOM.render(element, document.getElementById('root'));
}

setInterval(tick, 1000);
```

# Tailwind CSS

- Building complex components from a constrained set of primitive utilities.

- Using utility classes to build custom designs without writing CSS

- Why not just use inline styles? Designing with constraintsand Responsive design.

resourses 

[this toturial](https://reactjs.org/docs/hello-world.html)
[tailwindcss](https://tailwindcss.com/docs/utility-first)