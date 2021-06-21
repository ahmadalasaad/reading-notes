# HTML

## Text

In this chapter we focus on how to add markup to the text that appears on your pages. You will learn about:

* Structural markup: the elements that you can use to describe both headings and paragraphs
* Semantic markup: which provides extra information; such  as where emphasis is placed in a sentence, that something  you have written 

is a quotation (and who said it), the meaning of acronyms, and so on.

### Headings

HTML has six "levels" of headings
``` 
<h1>
<h2>
<h3>
<h4>
<h5>
<h6>
 
```

```<h1>``` is used for main headings

```<h2>``` is used for subheadings

If there are further sections  under the subheadings then the <h3> element is used, and so on..

### Paragraphs

``` <p> ```

To create a paragraph, surround  the words that make up the  paragraph with an opening ```<p>```

tag and closing </p> tag.

*By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs.*

### Bold & Italic

```<b>```

By enclosing words in the tags ```<b>``` and ```</b>``` we can make characters appear bold.

The ```<b>``` element also represents a section of text that would be presented in a visually different way (for example key words in a 

paragraph) although the use of the ```<b>``` element does not imply any additional meaning.

```<i>```

By enclosing words in the tags ```<i>``` and ```</i>``` we can make characters appear italic.

The ```<i>``` element also represents a section of text that would be said in a different way from surrounding content — such as 

technical terms, names of ships, foreign words, thoughts, or other terms that would usually be italicized.

### Superscript & Subscrip

```<sup>```

The ```<sup>``` element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts

 like raising a number to a power such as 2^2.

```<sub>```

The ```<sub>``` element is used to  contain characters that should be subscript. It is commonly used with foot notes or chemical 

formulas such as H2O .

### White Space

In order to make code easier to  read, web page authors often add extra spaces or start some elements on new lines.

When the browser comes across two or more spaces next to each other, it only displays one space. 

Similarly if it comes across a line break, it treats that as a single space too. This is known as **white space collapsing**.

### Line Breaks & Horizontal Rules

```<br />```

As you have already seen, the browser will automatically show each new paragraph or heading 

on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag ```<br />```.

```<hr />```

To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between 

sections using the ```<hr />``` tag.There are a few elements that do not have any words between an opening and closing tag. They 

are known as empty elements and they are written differently .An empty element usually has only one tag. Before the closing angled 

bracket of an empty element there will often be a space and a forward slash character. Some web page authors miss this out but it is a 

good habit to get into.


# CSS

## Introducing CSS

### Understanding CSS: Thinking Inside the Box

The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element.

CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

### CSS Associates Style rules with HTML elements

CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS 

rule contains two parts: a selector and a declaration .

### CSS Properties Affect How Elements Are Displayed

CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can 

specify several properties in one declaration, each separated by a semi-colon.


### You can use CSS in 3 ways:
 * External CSS
 * Iternal CSS
 * Inline CSS

### Why use External Style Sheets?

 All of your web pages can share the same style sheet. 

Therefore, once the user has downloaded the CSS stylesheet, the rest of the site will load faster. If you want to make a change to how 

your site appears, you only need to edit the one CSS file and all of your pages will be updated. For example, you can change the style 

of every ```<h1>``` element by altering the one CSS style sheet, rather than changing the CSS rules on every page. The HTML code will beeasier 

to read and edit because it does not have lots of CSS rules in the same document. It is generally considered good practice to have the 

content of the site separated from the rules that determine how it appears.

# JS

## Basic JavaScript Instructions

### STATEMENTS 

A script is a series of instructions that a computer can follow one-by-one. 

Each individual instruction or step is known as a statement. 

Statements should end with a semicolon.


JAVASCRIPT IS CASE SENSITIVE

JavaScript is case sensitive so hourNow means something different to HourNow or HOURNOW. 

STATEMENTS ARE INSTRUCTIONS AND EACH ONE STARTS ON A NEW LINE

A statement is an individual instruction that the computer should follow. Each one should start on a new line and end with a semicolon. 

This makes your code easier to read and follow.

STATEMENTS CAN BE ORGANIZED INTO CODE BLOCKS

Some statements are surrounded by curly braces; these are known as code blocks. The closing curly brace is not followed by a semicolon.

### COMMENTS

You should write comments to explain what your code does. 

They help make your code easier to read and understand. 

This can help you and others who read your code. 

```
/* This script displays a greeting to the user based upon the current time. 
It is an example from JavaScript & jQuer y book */
var today= new Date(); // Create a new data  object 
var hour Now = today.getHours(); //Find the current hour
var greeting; 
// Display the appropriate greeti ng based on the current time 
if (hourNow > 18) { 
greeting = 'Good evening ' ; 
else if (hourNow > 12) { 
greeting = 'Good afternoon'; 
else if (hourNow > 0) { 
greeting= ' Good morning'; 
else { 
greeting = 'Welcome'; 
} 
document.write(greeting) ; 

```

MULTI-LINE COMM ENTS 

To write a comment that stretches over more than one line, you use a multi-line comment, starting with the ```/* characters and ending 
with the */``` characters. 

Anything between these characters is not processed· by the JavaScript interpreter. 

SINGLE-LINE COMMENTS 

In a single-line comment, anything that follows the two forward slash characters // on that line will not be processed by the JavaScript 

interpreter. 

Singleline comments are often used for short descriptions of what the code is doing. 

### WHAT IS A VARIABLE?

A script will have to temporarily store the bits of information it needs to do its job. It can store this data in **variables**.

### DATA TYPES 

* NUMERIC DATA TYPE 

The numeric data type handles numbers. (0.75,2,0)

* STRING DATA TYPE 

The strings data type consists of letters and other characters. ('H. 1 ' )

* BOOLEAN DATA TYPE 

Boolean data types can have one of two values: true or false. (true,false)


### operators

**JavaScript has the following types of operators:**

* Assignment operators

```x = y , x = x + y , x = x - y , x = x * y , x = x / y``` ,.... 

* Comparison operators

```x == y , x < y , x > y , x >= y , x <= y```  

* Arithmetic operators

```x % y , x++ , x--``` , ...

* Bitwise operators

```x&y ,x|y , ~x ```, ....

* Logical operators

```x&&y , x||y , !X```

* String operators

``` 'x ' + 'y'```

* Conditional (ternary) operator

``` var status = (age >= 18) ? 'adult' : 'minor';``` 

* Comma operator


* Unary operators

* Relational operators

## Decisions and Loops

### SWITCH STATEMENTS 

A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code 

that should run if the variable matches that value. 

```
switch (level) { 
case 'One ': 
title= 'Level 1 ' ; 
break; 
case 'Two': 
tit 1 e = ' Level 2 ' ; 
break; 
case ' Three' : 
title = 'Level 3' ; 
break ; 
default : 
title= 'Test'; 
break; 
}

```