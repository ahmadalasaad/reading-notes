# Functions

Functions are one of the fundamental building blocks in JavaScript. A 

function in JavaScript is similar to a procedure—a set of statements 

that performs a task or calculates a value, but for a procedure to 

qualify as a function, it should take some input and return an output 

where there is some obvious relationship between the input and the 

output. To use a function, you must define it somewhere in the scope 

from which you wish to call it.

## there is to ways to define a function : 

### Function declarations
 
 you can define a declarations function  :
 
 
 function addOne(x) {
 
  return x+1;

}
 
 and then you should invoke the function :

 addOne(5);

 ### Function expressions

you can define an expressions function :
 
const addTwo = function(i) { 
  
  return i+2 ;
  
   }

and then you should invoke the function :

var x = square(4); 