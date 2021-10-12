1. Understanding the problem domain is the hardest part of programming
   - Make the problem domain easier
   - Get better at understanding the problem domain
2. What’s the difference between primitive values and object references in JavaScript?
   - JS 8 Data Types: Boolean, Null, Undefined, Number, BigInt, String, Symbol, **Objects [Arrays, functions, dates]**
   - When a primitive value is assigned to a variable (eg let foo = ‘bar’), the variable is set to that **value** directly. **IMMUTABLE**
   - When the variable is assigned with an object, however, things are different. Instead of containing the value directly, that variable contains a **reference**.
   - const moe = {name: 'Moe Szyslak'}
   - Object references/memory addresses are **MUTABLE** 


   - Strings are **IMMUTABLE** but can be reassigned
     - let word = 'snow', word[0] = 'k' WON'T WORK
   - Arrays are **MUTABLE** 
     - let letters = ['s', 'n', 'o', 'w']
     - letters[0] = 'k'
     - console.log(letters) // (4) ["k", "n", "o", "w"]
   - If you want to create a new object instead of a second reference to the same object (as we did above), you should use **Object.assign** instead. let coLead = Object.assign({}, lead, {name: 'Paul McCartney'})


     - let lead = 'John Lennon'
       - let coLead = lead
       - coLead = 'Paul McCartney'
       - console.log(lead, coLead) // John Lennon Paul McCartney
     - let lead = {
       - name: 'John Lennon',
       - group: 'The Beatles'
       - }
       - let coLead = lead
       - coLead.name = 'Paul McCartney'
       - console.log(lead, coLead)
       - // {name: "Paul McCartney", group: "The Beatles"} is **logged twice**

   - The loose equality operator (==) will return true if the values of the two items being compared are the same. The strict equality operator (===) returns true if the values and types of the two objects being compared are the same. 
   - Object references, on the other hand, do not contain values directly — they contain references. This causes equality checks with objects to give results that may not be intuitive to new developers.
   - In order to check whether the contents (not the reference) of two objects are the same you need to either:
       - Iterate through the object and check that each key and value match. This can be tricky because an object’s property can be an object in itself.
       - Convert the object to a suitable primitive before doing the equality check.
  
# JS
>Chapter 3: “Object Literals” (pp.100-105)
>Chapter 5: “Document Object Model” (pp.183-242)

- Browser, Web Server, Database
- document.write9) vs element.innterHTMl advantages and disadvantages (p 227)
- Selecting an element from a nodelist
  1. item() method -- var item = elements.item(0);
  2. array syntax -- var item = elements[0];