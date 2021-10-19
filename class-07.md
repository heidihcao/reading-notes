> Domain Modeling
1. https://github.com/codefellows/domain_modeling#domain-modeling
2. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
3. Model its attributes with a constructor function that defines and initializes properties.
4. Model its behaviors with small methods that focus on doing one job well.
5. Create instances using the new keyword followed by a call to a constructor function.
6. Store the newly created object in a variable so you can access its properties and methods from outside.
7. Use the this variable within methods so you can access the object's properties and methods from inside.

> HTML: Tables (pp.126-145)
1. <table>
2. <tr>: start of each row
3. <td>: each cell of a table
4. <th> just like <td> but its purpose is to represent the heading for a column or row.
5. Long tables: <thead> <tbody> <tfoot>
6. 

> JS: Functions, Methods, and Objects (pp.106-144)
## Under the hood, ARRAYS AND FUNCTIONS are Objects ## 
1. Storing data: variables; arrays; individual objects; multiple objects
2. Arrays of objects & Objects of array
3. Object model: a group of objects
   1. Browser Object Model
   2. Document Object Model (DOM)
   3. Global Javascript Objects

> Class notes
> ? Trailing Comma
> ? Prototype but overwrite one value?
>
'use strict';

//console.log('Hi');

// //object literal
// let oneStudent = {
//   name:'Steve', 
//   codeClass: 201,
//   pronouns: 'they, them',
//   online: true,
//   school: 'Code Fellows',
// };

// console.log(oneStudent);

// let otherStudent = {
//   name:'Juan', 
//   codeClass: 201,
//   pronouns: 'He, Him',
//   online: true,
//   school: 'Code Fellows'
// };

// console.log(oneStudent);

let studentArray = [];

// Constructor Function
//this. does not refer to Function, but the object that will be created "juan, sara"

function Student(name, pronouns){
  this.studentName = name;
  this.codeClass= 201;
  this.pronouns = pronouns;
  this.online = true;
  this.introduce = function(){
    console.log(`Hi my name is ${this.studentName}. My pronouns are ${this.pronouns}. I am in the ${this.codeClass}.`);
  };
  studentArray.push(this);
}

// Instantiate a Student object from a Constructor
let juan = new Student('Juan','he, him');
let sara = new Student('Sara', 'she, her');
// console.log(juan);
// console.log(sara);
// juan.introduce();
// sara.introduce();

console.log(studentArray);

// Student all inheriting the haircolor.
Student.prototype.hairColor = 'black';


for (let i=0; i < studentArray.length; i++){
  studentArray[i].introduce();
}