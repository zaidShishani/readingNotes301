# React Docs - Forms

## Reading questions :

1. What is a ‘Controlled Component’?

    It is a convenient way for JavaScript function to handle the submission of the form and has access to the data that the user entered into the form. 
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

3. How do we target what the user is entering if we have an event handler on an input field?
we use 
    ```
    event.target.value
    ```
    to target teh value from an event handler

## The Conditional (Ternary) Operator Explained

1. Why would we use a ternary operator?
    It allows us to assign one value to the variable if the condition is true, and another value if the condition is false and make the assignment of a value to a variable easier to see, because it's contained on a single line instead of an if else block.
    
2. Rewrite the following statement using a ternary statement:
    ```
    if(x===y){
    console.log(true);
    } else {
    console.log(false);
    }
    ```
    Rewritten
    ```
    console.log(x===y ? true : false;);
    ```