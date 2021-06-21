# LISTS

There are lots of occasions when we need to use lists. HTML provides us with three different types:

* Ordered lists are lists where each item in the list is numbered. For example, the list might be a set of steps for a recipe that must 

  be performed in order, or a legal contract where each point needs to be identified by a section number.
```
<ol>
<li>Chop potatoes into quarters</li>
<li>Simmer in salted water for 15-20
 minutes until tender</li>
<li>Heat milk, butter and nutmeg</li>
<li>Drain potatoes and mash</li>
<li>Mix in the milk mixture</li>
</ol>
```


* Unordered lists are lists that begin with a bullet point (rather than characters that indicate order).

```
<ul>
<li>1kg King Edward potatoes</li>
<li>100ml milk</li>
<li>50g salted butter</li>
<li>Freshly grated nutmeg</li>
<li>Salt and pepper to taste</li>
</ul>
```

* Definition lists are made up of a set of terms along with the definitions for each of those terms.

```
<dl>
<dt>Sashimi</dt>
<dd>Sliced raw fish that is served with 
 condiments such as shredded daikon radish or 
 ginger root, wasabi and soy sauce</dd>
<dt>Scale</dt>
<dd>A device used to accurately measure the 
 weight of ingredients</dd>
<dd>A technique by which the scales are removed 
 from the skin of a fish</dd>
<dt>Scamorze</dt>
<dt>Scamorzo</dt>
<dd>An Italian cheese usually made from whole 
 cow's milk (although it was traditionally made 
 from buffalo milk)</dd>
</dl>

```

# BOXES

## Border, Margin & Padding

Every box has three available properties that can be adjusted to control its appearance :

1. Border 

Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from 

another.

2. Margin

Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.

3. Padding

Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its 

contents.

# Decisions and Loop

 ## LOOPS

 ### for

 A for loop is often used to loop through the items in an array. 

In this example, the scores for each round of a test are stored in an array called scores. 

The total number of items in the array is stored in a variable called arrayl ength. This number is obtained using the l ength property 

of the array. There are three more variables: 

roundNumber holds the round of the test; msg holds the message to display; i is the counter (declared outside the loop). 

The loop starts with the for keyword, then contains the condition inside the parentheses. 

As long as the counter is less than the total number of items in the array, the contents of the curly braces will continue to 

run. Each time the loop runs, the round number is increased by 1. 

Inside the curly braces are rules that write the round number and the score to the msg variable. The variables declared outside of the 

loop are used within the loop. 

The msg variable is then written into the page. It contains HTML so the i nnerHTML property is used to do this. Remember, p228 will talk 

about security issues relating to this property. 

```
var scores= [24. 32, 17]; //Array of scores 
var arraylength scores.l ength; // Items in array 
var roundNumber = O; //Current round 
var msg ''; //Message 
var i ; // Counter 
//Loop through the items in the array 
for (i = O; i < arraylength; i++) { 
//Arrays are zero based (so 0 is round 1) 
//Add 1 to the current round 
roundNumber = (i + l); 
// Write the current round to message 
msg += 'Round ' + roundNumber + ' : '; 
//Get the score from the scores array 
msg += scores[i] + '<br / >' ; 
document .getElementByid( 'answer') .i nnerHTML msg;
```

### while

Here is an example of awhil e loop. It writes out the 5 times 

table.

 Each time the loop is run, another calculation is written into the variable called msg. 

This loop will continue to run for as long as the condition in 

the parentheses is true. 

That condition is a counter indicating that, as long as the variable 

i remains less than 10, the statements in the subsequent code block should run. 

Inside the code block there are two statements: 

The first statement uses the+= operator, which is used to add 

new content to the msg variable.

Each time the loop runs, a new calculation and line break is added to the end of the message being stored in it. So+" works as 

a shorthand for writing: 

msg = msg + 'new msg' 

(See bottom of the next page for a breakdown of this statement.) The second statement increments the counter variable 

by one. (This is done inside the loop rather than with the condition.)

When the loop has finished, the interpreter goes to the next line of code, which writes the msg variable to the page.

```
var i = l ; 
var msg = ' ' ; 
II Set counter to 1 
II Message 
II Store 5 times tabl e in a variable 
while (i < 10) { 
msg += i + ' x 5 = ' + (i * 5) + '<br I>'; 
i++; 
document .getEl ementByid( ' answer') . innerHTML = msg;

```

### DO WHILE

The key difference between a while loop and a do while loop is that the statements in the code block come before the condition. This 

means that those statements are run once whether or not the condition is met.

If you take a look at the condition, it is checking that the value of the variable called i is less than 1, but that variable has 

already been set to a value of 1.

Therefore, in this example the result is that the 5 times table is written out once, even though the counter is not less than 1. 

Some people like to write while on a separate line from the closing curly brace before it.

```
var i = l;  // Set counter to 1 
var msg ='' // message
// Store 5 times table in a variable 
do { 
msg += i + ' x 5 = ' + (i * 5) + '<br I>' ;s 
i++; 
} wh il e ( i < 1) ; 
// Note how this is already 1 and it still runs 
document .getEl ementByld(' answer').innerHTML = msg; 

```