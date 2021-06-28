# Layout

* **Controlling the Position of Elements**

CSS has the following positioning schemes that allow you to control 
the layout of a page: normal flow, relative positioning, and absolute 
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.


Normal flow

Every block-level element 
appears on a new line, causing 
each item to appear lower down 
the page than the previous one. 
Even if you specify the width 
of the boxes and there is space 
for two elements to sit side-byside, they will not appear next 
to each other. This is the default 
behavior (unless you tell the 
browser to do something else).

```
html
<body>
<h1>The Evolution of the Bicycle</h1>
<p>In 1817 Baron von Drais invented a walking 
 machine that would help him get around the 
 royal gardens faster...</p>
</body>

css

body {
width: 750px;
font-family: Arial, Verdana, sans-serif;
color: #665544;}
h1 {
background-color: #efefef;
padding: 10px;}
p {
width: 450px;}
````
Relative Positioning

This moves an element from the 
position it would be in normal 
flow, shifting it to the top, right, 
bottom, or left of where it 
would have been placed. This 
does not affect the position of 
surrounding elements; they stay 
in the position they would be in 
in normal flow.

```
html
<body>
<h1>The Evolution of the Bicycle</h1>
<p>In 1817 Baron von Drais invented a walking 
 machine that would help him get around the 
 royal gardens faster...</p>
</body>

css
p.example {
position: relative;
top: 10px;
left: 100px;}
```
Absolute positioning

This positions the element 
in relation to its containing 
element. It is taken out of 
normal flow, meaning that it 
does not affect the position 
of any surrounding elements 
(as they simply ignore the 
space it would have taken up). 
Absolutely positioned elements 
move as users scroll up and 
down the page.

``` 
html
<body>
<h1>The Evolution of the Bicycle</h1>
<p>In 1817 Baron von Drais invented a walking 
 machine that would help him get around the 
 royal gardens faster...</p>
</body>

css

h1 {
position: absolute;
top: 0px;
left: 500px;
width: 250px;}
p {
width: 450px;}

```


To indicate where a box should be positioned, you may also need to use 
box offset properties to tell the browser how far from the top or bottom 
and left or right it should be placed.

Fixed Positioning 

This is a form of absolute 
positioning that positions 
the element in relation to the 
browser window, as opposed 
to the containing element. 
Elements with fixed positioning 
do not affect the position of 
surrounding elements and they 
do not move when the user 
scrolls up or down the page.

```
html

<body>
<h1>The Evolution of the Bicycle</h1>
<p class="example">In 1817 Baron von Drais 
 invented a walking machine that would help him 
 get around the royal gardens faster...</p>
</body>

css

h1 {
position: fixed;
top: 0px;
left: 50px;
padding: 10px;
margin: 0px;
width: 100%;
background-color: #efefef;}
p.example {
margin-top: 100px;}

```


Floating Elements

Floating an element allows 
you to take that element out 
of normal flow and position 
it to the far left or right of a 
containing box. The floated 
element becomes a block-level 
element around which other 
content can flow.

```
html

<h1>The Evolution of the Bicycle</h1>
<blockquote>"Life is like riding a bicycle.
 To keep your balance you must keep moving." - 
 Albert Einstein</blockquote>
<p>In 1817 Baron von Drais invented a walking 
 machine that would help him get around the royal 
 gardens faster: two same-size in-line wheels, the 
 front one steerable, mounted in a frame ... </p>

css

blockquote {
 float: right;
 width: 275px;
 font-size: 130%;
 font-style: italic;
 font-family: Georgia, Times, serif;
 margin: 0px 0px 10px 10px;
 padding: 10px;
 border-top: 1px solid #665544;
 border-bottom: 1px solid #665544;}
 
```


 