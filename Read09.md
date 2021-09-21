# Reading questions :


## Functional Programming Concepts

1. What is functional programming?
    >Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

2. What is a pure function and how do we know if something is a pure function?
    it is onme of the first fundamental concept we learn when we want to understand and to know if some thing is a pure functions we look for 
    * It returns the same result if given the same arguments (it is also referred as deterministic)
    * It does not cause any observable side effects

3. What are the benefits of a pure function?
    1. immediately testable. 
    2. maintaining and refactoring code much easier.
    3. better quality code.


4. What is immutability?
    It means Unchanging over time or unable to be changed. that its state cannot change after it’s created.

5. What is Referential transparency?
    it is when a function consistently yields the same result for the same input.


## Node JS Tutorial for Beginners #6 - Modules and require(

1. What is a module?
    is a set component containing 1 or more funcations

2. What does the word ‘require’ do?
    it imports data from it's given path

3. How do we bring another module into the file the we are working in?
    We use require and give it a verable and equal it to whater the module exports from the other file

4. What do we have to do to make a module available?
    we have to export the module function