# React: Passing Functions as Props


## Reading questions :


### React Docs - lists and keys

1. What does .map() return? 

    return a new array with each element results from the callback 

2. If I want to loop through an array and display each value in JSX,  how do I do that in React?

    We can use .map() or forEach () funcation

3. Each list item needs a unique Key.

4. What is the purpose of a key?
    React uses keys to identify changed, added or removed items.

***
### The Spread Operator

1. What is the spread operator?
    The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.
2. List 4 things that the spread operator can do.
    1. Copying an array
    2. Concatenating or combining arrays
    3. Using Math functions 
    4. Using an array as arguments
3. Give an example of using the spread operator to combine two arrays.
    ```
    const myArray = [`🤪`,`🐻`,`🎌`]
    const yourArray = [`🙂`,`🤗`,`🤩`]
    const ourArray = [...myArray,...yourArray]
    console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩
    ```
4. Give an example of using the spread operator to add a new item to an array.
    ```
    const fewFruit = ['🍏','🍊','🍌']
    const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
    console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]
    ```
5. Give an example of using the spread operator to combine two objects into one.
    ```
    const objectOne = {hello: "🤪"}
    const objectTwo = {world: "🐻"}
    const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
    console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
    const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
    objectFour.laugh() // 😂😂😂😂😂
    ```
***

