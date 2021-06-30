# Error Handling & Debugging

When you are writing JavaScript, do not expect to write it perfectly the first time. 
Programming is like problem solving: you are given a puzzle and not only do you have to solve 
it, but you also need to create the instructions that allow the computer to solve it. too.

* **HOW TO DEAL WITH ERRORS**

1- DEBUG THE SCRIPT TO FIX ERRORS 
If you come across an error while writing a script 
(or when someone reports a bug), you will need to 
debug the code, track down the source of the error, 
and fix it. 

You will find that the developer tools available in 
every major modern browser will help you with 
this task. In this chapter, you will learn about the 
developer tools in Chrome and Firefox. (The tools in 
Chrome are identical to those in Opera.) 

2- HANDLE ERRORS GRACEFULLY 
You can handle errors gracefully using try, catch, 
throw, and f i na 1 ly statements. 

Sometimes, an error may occur in the script for a 
reason beyond your control. For example, you might 
request data from a third party, and their server 
may not respond. In such cases, it is particularly 
important to write error-handling code.

* **HANDLING EXCEPTIONS**

If you know your code might fail, use try, catch, and finally. 
Each one is given its own code block. 

```

try { 
II Try to execute this code 
catch (exception) { 
II If there is an exception, run this code 
fina lly { 
II This always gets executed
}

```

TRY

First, you specify the code 
that you think might throw an 
exception within the try block. 

If an exception occurs in this 
section of code, control is 
automatically passed to the 
corresponding catch block. 

The try clause must be used in 
this type of error handling code, 
and it should always have either 
a catch, fi na 1 ly, or both. 

If you use a continue, break, or 
return keyword inside a try, it 
will go to the f i na 11 y option

CATCH 

If the try code block throws an 
exception, catch steps in with an 
alternative set of code. 

It has one parameter: the error 
object. Although it is optional, 
you are not handling the error if 
you do not catch an error.

he ability to catch an error can 
be very helpful if there is an issue 
on a live website. 

It lets you tell users that 
something has gone wrong 
(rather than not informing them 
why the site stopped working). 

FINALLY

The contents of the fi na 11 y 
code block will run either 
way - whether the try block 
succeeded or failed. 

It even runs if a return keyword 
is used in the try or catch block. 
It is sometimes used to clean up 
after the previous two clauses. 

You can nest checks inside each 
other (place another t ry inside a 
catch), but be aware that it can 
affect performance of a script.


