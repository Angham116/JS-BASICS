# JS-BASICS 

 ## Object.assign : 
    method is used to copy the values of all enumerable 
    own properties from one or more source objects to a target object. It will return the target object.
    
 - e.g :  
   ```javascript 
     const target = { a: 1, b: 2 };
         const source = { b: 4, c: 5 };
         const returnedTarget = Object.assign(target, source);

        console.log(target);
        // expected output: Object { a: 1, b: 4, c: 5 }

        console.log(returnedTarget);
        // expected output: Object { a: 1, b: 4, c: 5 }
   ```


## Spread Operator
   ```javascript
     const target = { a: 1, b: 5, c:7 };
     const spread = {...target};
     console.log(spread);  // will return spread = { a: 1, b: 5, c:7 }; as a copy of target
   ```
