# React Docs - Thinking in React

## Reading questions :

1. What is the **single responsibility principle** and how does it apply to components?

    Is that a component should one thing if it does more we sohuld split it into smaller subcomponents.

2. What does it mean to build a ‘static’ version of your application?

    means building a verion of the application that only render data props and will not be interactive meaning there is no state.

3. Once you have a static application, what do you need to add?

    we need to be able to trigger the underlying data model we can achieves this with state, we also need minimal representation of the state your application needs and compute everything else you need on-demand. 

4. What are the three questions you can ask to determine if something is state?
    1. Is it passed in from a parent via props? If so, it probably isn’t state ?
    2. Does it remain unchanged over time? If so, it probably isn’t state ?
    3. Can you compute it based on any other state or props in your component? If so, it isn’t state ?


5. How can you identify where state needs to live?

    > we follow these steps:
    >* Identify every component that renders something based on that state.
    >* Find a common owner component (a single component above all the components that need the state in the hierarchy).
    >* Either the common owner or another component higher up in the hierarchy should own the state.
    >* If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

***

# Higher-Order Functions

## Reading questions :

1. What is a “higher-order function”?

    > Functions that operate on other functions, either by taking them as arguments or by returning them.

2. Explore the **greaterThan** function as defined in the reading. In your own words, what is line 2 of this function doing?
    ```
    return m => m > n;
    ```
    it's running arrow function to return the comparison of ```m``` and ```n```

3. Explain how either map or reduce operates, with regards to higher-order functions.

    with reduce operates we take for the parameters the array , combining function and starting value. the standard array method reduce, which corresponds this function, has a convenience that if our array contains at least one element we are allowed to leave off start argument the method will take the first element of the array as its start value and start reducing at the second element.

    code example:
    ```
    function reduce(array, combine, start) {
    let current = start;
    for (let element of array) {
        current = combine(current, element);
    }
    return current;
    }

    console.log(reduce([1, 2, 3, 4], (a, b) => a + b, 0));
    // → 10
    ```