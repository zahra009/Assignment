ONE:
* Arguments objects are not available in arrow functions, but are available in regular functions.
* Regular functions created using function declarations or expressions are 'constructible' and 'callable' while the arrow functions are only ‘callable’ and not constructible. 

arrow function(let x = ()=> {
    console.log(arguments);
};
new x(1,2,3);)

regular function(let x = function(){
    console.log(arguments);
};
new x =(1,2,3);)

TWO:
console.log(test);   // undefined
var test;
greet();

function greet() {
    console.log('Hi, there.');
}

THREE:
Pure functions return the same output if we use the same input parameters. However, impure functions give different outcomes when we pass the same arguments multiple times.

A pure function is always predictable and has no side effects. An impure function is unpredictable and has side effects.