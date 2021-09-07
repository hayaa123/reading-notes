# React Docs - lists and keys

## What does .map() return?

map function loop over an array and take a function to operate in the array and return modified version of it 

## If I want to loop through an array and display each value in JSX, how do I do that in React?

we can use map and put the wanted output component inside of it as a funtion and return the outputs using curly brackets 

```
arr.map(item=>{
    <component propariety1 ={item} />
})
```

## Each list item needs a unique id.


## What is the purpose of a key?

helps identify wich item has changed 


# The Spread Operator

## What is the spread operator?

refer to the use of three dots `...`

in functional call when `...arr` used it expand an iterable object to the list of argument 

eg :

```
Math.max(...[1,3,5]) // 5
```

## List 4 things that the spread operator can do.

1- copieng an array

2- using Math functions

3-adding item to a list

4-adding t state in react

## Give an example of using the spread operator to combine two arrays.

```
arr1= [1,2,3,4]
arr2=[5,6,7,8]

arr3 = [...arr1,...arr2]

```

## Give an example of using the spread operator to add a new item to an array.

```
arr = [1,2,3,...arr1]
```

## Give an example of using the spread operator to combine two objects into one.

```
obj1 = {key1:value1}
obj2 = {key2:value2}
obj3 = {...obj1,...obj2}
```