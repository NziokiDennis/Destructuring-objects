# Destructuring-objects
let person = {
 name: 'Bob',
 age: 25
};
let { name, age } = person;
// Is equivalent to
let name = person.name; // 'Bob'
let age = person.age; // 25
Destructuring and renaming:
let person = {
 name: 'Bob',
 age: 25
};
let { name: firstName } = person;
// Is equivalent to
let firstName = person.name; // 'Bob'
Destructuring with default values:
let person = {
 name: 'Bob',
 age: 25
};
let { phone = '123-456-789' } = person;
// Is equivalent to
let phone = person.hasOwnProperty('phone') ? person.phone : '123-456-789'; // '123-456-789'
