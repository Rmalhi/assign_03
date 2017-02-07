CLOSURES:
As the word closure itself is able to clear its meaning, a closure “closes over” the free variables of a function. A variable is said to be free when its declaration is not made within a function means it comes from outside. A closure being an inner function has easy access to the outer functions along with its own variables and global variables. A closure can be created by adding a function in another function. In the javascript , the inner functions have complete access to all variables plus functions defined inside the outer functions. But, for the outer variables, its vice-versa as they don’t have any access to variables and functions defined inside inner function. Moreover, a closure can be described as a function and the connection to the scope in which the function is created. Whenever we use function inside another function a closure is used.
A closure can be declared as:
var car=function(name){  // The outer function defines a variable called “name”
var getName=function(){
return name;  //The inner function has access to “name” variable of outer function
}
Return getName; //Returns the inner function  exposing it to outer scope
};
myCar=car (“Scoda”);
myCar(); //Returns “Scoda”

References:
https://www.youtube.com/watch?v=HjJQ-lvTgWg

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions#Closures

http://eloquentjavascript.net/05_higher_order.html

http://stackoverflow.com/questions/111102/how-do-javascript-closures-work?rq=1
