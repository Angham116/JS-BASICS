

## JS-BASICS 

 ### * Object.assign: 
 
  ##### method is used to copy the values of all enumerable own properties from one or more source objects to a target object. It will return the target object.
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


### * Spread Operator:

   ##### The spread operator allows an iterable to spread or expand individually inside a receiver. Iterables are anything that can be looped over such as strings, arrays, and sets.
   ```javascript
     const target = { a: 1, b: 5, c:7 };
     const spread = {...target};
     console.log(spread);  // will return spread = { a: 1, b: 5, c:7 }; as a copy of target
   ```
  
  
### * Deep Clone
    
   ##### For deep cloning, we need to use other alternatives because Object.assign() copies property values. If the source     value is a reference to an object, it only copies that reference value.
   ```javascript
       obj1 = { a: 0 , b: { c: 0}};
       let obj3 = JSON.parse(JSON.stringify(obj1));
       obj1.a = 4;
       obj1.b.c = 4;
        console.log(JSON.stringify(obj3)); // { a: 0, b: { c: 0}}
   ```
   
   ### 
 ```javascript 
     const condition = authUser => authUser != null;

    // same with this short version
     const condition = authUser => !!authUser;
 ```
