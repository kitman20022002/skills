# Hoisting

## PRIOR KNOWLEDGE
 - function expression 
 - class expression
 - function
 - variables
 - classes

## Key points:
- Hoisiting: a process where the **interpreter declares** one of the following **functions variables or classes  before** the **code executes**

- Benfits
  - Let you to use a function before you declare it in your code 

- How does hositing work
  - The Interpreter builds a tree (AST) to declare all the **functions** , **variables**, **classes** and assign a default value before the code get executed  

- Three types of hoisiting
  - functions hoisiting
  - variables hoisiting
  - classes hoisiting

## Benfits
As mentions above one of the advantages of hoisting is that it lets you use a function before you declare it in your code. Example: We can call catName before the function has been decleared
```
catName("Tiger");

function catName(name) {
  console.log("My cat's name is " + name);
}
/*
The result of the code above is: "My cat's name is Tiger"
*/
```
Without hoisting you would have to write the same code like this:
```
function catName(name) {
  console.log("My cat's name is " + name);
}

catName("Tiger");
/*
The result of the code above is the same: "My cat's name is Tiger"
*/
```

## Function hoisting
We can call catName before the function has been decleared
```
catName("Tiger");

function catName(name) {
  console.log("My cat's name is " + name);
}
/*
The result of the code above is: "My cat's name is Tiger"
*/
```

## Varaible hositing
We can call catName before the varabiles has been decleared

## Class hositing


## Misunderstanding Concpts
- **function expression** in **not hoisted**
- **class expression** in **not hoisted**
- Hoisting **does not move the decleation** up to the **top of the JS file** 
