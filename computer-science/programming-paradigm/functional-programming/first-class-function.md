# First Class Function

## PRIOR KNOWLEDGE
- argument

## Keypoints
- First-Class Function needs to match **one of following three Requiements**
  - Functions can be pass as arguments
  - You can the return a function from functions
  - Save them in variables.

function = first class objects

## Description
### Functions can be pass as arguments   = function a can be passed in b as a argument
```
function b(f){
}

function a(){

}

b(a)
```

### You can the return a function from functions = You can the return a function from functions = You can return a from b
```
function b(){
  return a();
}

function a(){

}

b(a)
```


### Save them in variables = = Save function in variable b
```
const b = function(){ 
  return a();
}

b(a)
```
