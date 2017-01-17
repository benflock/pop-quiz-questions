1. How do you delete a key value pair in an object?  i.e. delete firstName in the object:
var person = {
  firstName: "Bruce",
  lastName: "Wayne"
}

Expected answer: delete person.firstName;

2. How would you collect the keys of an object named "plans" in a variable named x?  What variable type will x be?

Expected answer: var x = Object.keys(plans);
x will be an array contains the key names as strings - i.e. [keyname1, keyname2,..]

3. How do you change var numObj = 12.345678 to 12.3?

Expected answer: numObj = numObj.toFixed(1);

4. What is type coercion?  What is the difference between explicit and implicit type coercion?  Give examples.

Expected answer: Type coercion is when the typeOf some variable changes as a result of some action taken.
 Explicit Type Coercion:
var a = "42";
var b = Number( a );
a;              // "42"
b;              // 42 -- the number!

Implicit Type Coercion:
var a = "42";
var b = a * 1;  // "42" implicitly coerced to 42 here
a;              // "42"
b;              // 42 -- the number!

5. How would you test if an object (i.e. var person = {name: "Watson"} has a particular key, i.e. "name"?

Expected answer: var x = person.hasOwnProperty("name");
x will = true if person has the property "name".
