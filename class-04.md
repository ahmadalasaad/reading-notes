# Links

Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of 

browsing or surfing.

* Links are created using the ```<a>``` element.

* The ```<a>``` element uses the href attribute to indicate the page you are linking to.

```
<a href="http://www.imdb.com">IMDB</a>
```



* If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.

```
<a href="reviews.html">Reviews</a>
```

* You can create links to open email programs with an email address in the "to" field.

```<a href="mailto:jon@example.org">Email Jon</a>```

* You can use the id attribute to target elements within a page that can be linked to.

```
<a href="http://www.imdb.com" target="_blank">

```

# Layout

* ```<div>``` elements are often used as containing elements to group together sections of a page.

* Browsers display pages in normal flow unless you 

specify relative, absolute, or fixed positioning.

* The float property moves content to the left or right of the page and can be used to create multi-column 

layouts. (Floated items require a defined width.)

* Pages can be fixed width or liquid (stretchy) layouts.

* Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its 

relevance without scrolling).

* Grids help create professional and flexible designs.

* CSS Frameworks provide rules for common tasks.

* You can include multiple CSS files in one page

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
 
 ```
 function addOne(x) {
 
  return x+1;

}
```
 
 and then you should invoke the function :

```
 addOne(5);
```

 ### Function expressions

you can define an expressions function :

``` 
const addTwo = function(i) { 
  
  return i+2 ;
  
   }

```

and then you should invoke the function :

```

var x = square(4); 

```

# Pair Programming

## How does pair programming work?

While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the 

programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the 

text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does 

not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be 

converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up 

solutions and documentation, but should not be writing any code.

## Why pair program?

1. Greater efficiency

It is a common misconception that pair programming takes a lot longer and is less efficient.

2. Engaged collaboration

When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were 

working alone.

3. Learning from fellow students

Everyone has a different approach to problem solving; working with a teammate can expose developers to techniques they otherwise would 

not have thought of.

4. Social skills

Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key.

5. Job interview readiness

A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or 

through a shared screen.

6. Work environment readiness

Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver 

a product.