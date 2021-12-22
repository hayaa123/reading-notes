# React

## Create a Next.js App

- Create a Next.js app

    `npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn/tree/master/basics/learn-starter"`

- Run the development server

    `npm run dev`

- Editing the Page
    - Make sure the Next.js development server is still running.
    Open pages/index.js with your text editor.
    Find the text that says “Welcome to” under the `<h1>` tag and change it to “Learn”. 
    - Save the file.
    - continueediting and adding youe elements 

you canfind examples repo [here](https://github.com/vercel/next.js/tree/canary/examples)


## React Context for Beginners

- What is React context?

    React context allows us to pass down and use (consume) data in whatever component we need in our React app without using props.

- When should you use React context?

    - React context is great when you are passing data that can be used in any component in your application.
    - Data should be placed on React context that does not need to be updated often.

- What problems does React context solve?

    React context helps us avoid the problem of props drilling.

    note : Props drilling is a term to describe when you pass props down multiple levels to a nested component, through components that don't need it.

    -There are four steps to using React context:

        1- Create context using the createContext  method.  
        export const UserContext = React.createContext();

        2- Take your created context and wrap the context provider around your component tree.

        3-Put any value you like on your context provider using the value prop.
        
        4- Read that value within any component by using the context consumer.

