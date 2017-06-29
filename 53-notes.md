##Javascript Lecture Notes

Q: Can curly braces wrap the body of a function on the same line?
A: Best practice is to put closing curly on a new line.

Q: How do you key into an object?
A: You can use brackets to key in via a variable, or . to key in with a actual key.

Q: Are floats and ints treated the same way?
A: Yes.

Q: Can you have more than one function in an object?
A: Yes, as many as you want.

Q: Syntax for defining a function in an object?
A: Various ways... 1. Start declaring the function and refer to it by name 2. Set function as a value for a key (name of the function)

Q: Are commas necessary in an object?
A: Yes, you need them to separate key value pairs.

Q: Why don't we need the function keyword?
A: You do, unless you're inside of an object.

Q: Where do prototypes come into play?
A: Prototypes are like Ruby classes. They tell you how to set up objects.

Q: Difference between const and let?
A: We'll talk about scoping in a minute, but they have the same effect.

Q: Are && and || lazily evaluated?
A: Yes, they are short-circuited.

Q: Are arrays ever equal with == ?
A: No.

Q: typeof "" ?
A: String.

Q: typeof back ticks ?
A: String.

Q: What does a fat arrow function look like?
A: (goes to whiteboard...can be declared anonymously, or be named)

Q: Difference between:
  function f() {}
  let f = function() {}
A: Nope

Q: Preferred approach?
A: In general, anything is fine. There are advantages to fat arrow, so you'll need to use it sometimes. I prefer to use it most of the time.

Q: NaN is always false?
A: Yes, it's one of 7 falsely values.

Q: Is there a difference between false and falsey?
A: Anything that evaluates to false is falsey.

Q: What is the prototype of a POJO?
A: Objects have __proto__ that point to object's prototype

Q: Can you explain __proto__ ?
A: You'll get more detail in a future lecture. It has to do with the way that JS gives objects behavior, and handles inheritance.
In JS, objects are created by constructor functions, and __proto__ points back to the constructor that created it.

Q: Prototype object vs POJOs?
A: Prototypes are functions. Objects are born from constructor functions. Objects have prototypes. Objects hold __proto__ as a reference to its prototype.

Q: Does Math.random always return a number between 0 and 1?
A: Yes.

Q: Can we concatenate numbers and strings?
A: Yes. It will coerce the number to a string. JS hates throwing errors.

Q: Prioritization of inheritance?
A: If the function is defined on the object, it will use it. If not, it will look to its prototype.

Q: Can you set default values on the prototype?
A: Better way to do it is to set default values on the constructor function. Use default arguments, same syntax as Ruby.

Q: How do we have access to a variable defined outside of a function?
A: Scoping! We have access to anything defined in the upper scope, because ... closures!

Q: Being a closure vs. having a closer?
A: A function is a closure, or a function closes over variables.

Q: Global and window are top-level objects?
A: Yes.

Q: Is window a function?
A: No. Window is an object.

Q: let vs. const?
A: const provides a guarantee that that variable will not be changed unintentionally.

Q: Can you close over variables that are multiple levels removed from you?
A: Yup!

Q: Do all functions have closures?
A: All functions will close over any variables available to them when they are declared, but you don't have to use any variables that you don't need.

Q: If we're okay with closures, why not var?
A: Var is about accessing something outside of where it's declared, closures go in the reverse direction.

Q: Why do you need to say this.property?
A: You must be explicit with this, unlike self in Ruby.

Q: This is available inside the prototype, and references an instance of the constructor?
A: Yes.

Q: Return vs print?
A: return and console.log are effectively the same in terms of output, in this example.

Q:
