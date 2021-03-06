# Closures

## PRIOR KNOWLEDGE
- Lexical environment

## Questions 
- What is Closures ? 
- How to create a Closures ? 
- What are the benfits of closures ? 

## Key points:

- Closures would need to match the following **Two Requiements**
    - **function bundled together**
    - **references** to its **surrounding state** (references to its surrounding state in JS = lexical environment) 
- Benfits
    - Closure gives you access to an outer function’s scope from an inner function


## Description 
Closures has to match **Two Requiements**

    - function bundled together
    - references to its surrounding state (references to its surrounding state in JS = lexical environment)
    
### Condition Example 
1. The combination of a function bundled together, which looks like following = **doStuff and abc are bundled together**
```
function doStuff() {
    function abc(){
        
    }
}
`````

2. References to its surrounding state in JS we use lexical environment = **abc can access the variable surroundingState**

```
function doStuff() {
    const surroundingState = 'hi'
    function abc(){
        console.log(surroundingState)
     }
}
//will output hi
```

### Code example 
Based a two requiements above a closures will look like below      

```
function doStuff() {
    const surroundingState = 'hi'
    function abc(){
        console.log(surroundingState)
     }
}
//will output hi
```

