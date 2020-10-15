# Refactoring - Functional Programming

## Concepts of Functional Programming in JS
What is functional programming?
- a style of building the structure and elements of computer programs and avoids changing-state and mutable data
    (wiki)

    *Pure Functions*
    - returns same result if given same arguments / deterministic
        - reading files... If our function reads files, it is impure since the file's contents can change
        - any function that relies on random # generation is impure 
    - does not cause any observable side effects
        - examples of *observable* side effects include changing a global object or a parameter passed for reference
    - benefits of pure functions --> the code is easier to test, you can expect the return value

    *Immutability*
    - unchanging over time or unable to be changed
    - when data is immutable, its *state cannot change after it is created*
        - to change it you must *create a new object with the new value*
        - handling mutability in iteration is known as **recursion**
            - this keeps variables immutable
    *Functions as first-class entities*
    - treated as *values* and *used as data*
        - able to refer from constants and variables, pass it as a parameter to other functions, and return it as a result from other functions
    *Filter*
    - expects a true or false value to determine if element should or should be included in the result collection
        - an example is when we only want even numbers from a collection of integers
    *Map*
    - to transform a collection
    - applies a function to all of its elements and builds a new collection from returned values
    *Reduce*
    - to receive a function and a collection, and then return a value created by combining the items

[<=Back](README.md)