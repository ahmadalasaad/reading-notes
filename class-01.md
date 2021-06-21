# HTML

HTML (Hypertext Markup Language) is the code that is used to 

structure a web page and its content. For example, content could be 

structured within a set of paragraphs, a list of bulleted points, or 

using images and data tables. As the title suggests, this article 

will give you a basic understanding of HTML and its functions.

## Structure

***HTML uses elements to describe the structure of Pages***

**The main parts of our element are as follows:**

* The opening tag: This consists of the name of the element (in this 

case, p), wrapped in opening and closing angle brackets. This states 

where the element begins or starts to take effect — in this case 

where the paragraph begins.

* The closing tag: This is the same as the opening tag, except that 

it includes a forward slash before the element name. This states 

where the element ends — in this case where the paragraph ends. 

Failing to add a closing tag is one of the standard beginner errors 

and can lead to strange results.

* The content: This is the content of the element, which in this case,

 is just text.

* The element: The opening tag, the closing tag, and the content 

together comprise the element.

### You can see the HTML code below

```
<html>

<head>

 <title>This is the Title of the Page</title>

</head>

<body>

 <h1>This is the Body of the Page</h1>

 <p>Anything within the body of a web page is

 displayed in the main browser window.</p>

</body>

</html>

```
## Extra Markup 

### DOCTYPES

Because there have beenseveral versions of HTML, eachweb page should 

begin with a DOCTYPE declaration to tell a browser which version of 

HTML the page is using (although browsers usually display the

page even if it is not included). 

HTML version | DOCTYPE
------------ | -------
HTML5        | ``` <!DOCTYPE html>```
HTML 4       | ```<!DOCTYPE html PUBLIC"-//W3C//DTD HTML 4.01 Transitional//EN""http://www.w3.org/TR/html4/loose.dtd">```
Transitional XHTML 1.0 | ```<!DOCTYPE html PUBLIC"-//W3C//DTD XHTML 1.0 Transitional//EN""http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"> ```
Strict XHTML 1.0 | ```<!DOCTYPE html PUBLIC"-//W3C//DTD XHTML 1.0 Strict//EN""http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">```
XML Declaration | ```<?xml version="1.0" ?>```

### Comment

If you want to add a comment to your code that will not be visible in the user's browser, you can add 

the text between these characters:
```
<!-- comment goes here -->
```

### ID attribute

Every HTML element can carry the id attribute. It is used to uniquely identify that element from other 

elements on the page. Its value should start with a letter or an underscore (not a number or any other 

character). It is important that no two

elements on the same page have the same value for their id attributes (otherwise the value is no 

longer unique).

**you can use id-attribute like this code below :**

```
<p>Water and air. So very commonplace are these
 substances, they hardly attract attention - and
 yet they vouchsafe our very existence.</p>
<p id="pullquote">Every time I view the sea I feel
 a calming sense of security, as if visiting my
 ancestral home; I embark on a voyage of seeing.
</p>
<p>Mystery of mysteries, water and air are right
 there before us in the sea.</p> 
 ```

 ### Class attribute

 
 Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one 
 
 element within a document, you will want a way to identify several elements as being different from 
 
 the other elements on the page. For example, you might have some paragraphs of text that contain 
 
 information that is more important than others and want to distinguish these elements, or you might 
 
 want to differentiate between links that point to other pages on your own site and links that point 
 
 to external sites.

 **you can use class-attribute like this code below :**

```
 <p class="important">For a one-year period from
 November 2010, the Marugame Genichiro-Inokuma
 Museum of Contemporary Art (MIMOCA) will host a
 cycle of four Hiroshi Sugimoto exhibitions.</p>
<p>Each will showcase works by the artist
 thematically contextualized under the headings
 "Science," "Architecture," "History" and
 "Religion" so as to present a comprehensive
 panorama of the artist's oeuvre.</p>
<p class="important admittance">Hours: 10:00 – 18:00
 (No admittance after 17:30)</p>

 ```

 ### iframe

 An iframe is like a little window that has been cut into your page — and in that window you can see 
 
another page. The term iframe is an abbreviation of inline frame.

```
<iframe
width="450"
height="350"
src="http://maps.google.co.uk/maps?q=moma+new+york
&amp;output=embed">
</iframe>

```
### meta

It is not visible to users but fulfills a number of purposes such as telling search engines about your 

page, who created it, and whether or not it is time sensitive. (If the page is time sensitive, it can 

be set to expire.)

```
<!DOCTYPE html>
<html>
<head>
 <title>Information About Your Pages</title>
 <meta name="description"
 content="An Essay on Installation Art" />
 <meta name="keywords"
 content="installation, art, opinion" />
 <meta name="robots"
 content="nofollow" />
 <meta http-equiv="author"
 content="Jon Duckett" />
 <meta http-equiv="pragma"
 content="no-cache" />
 <meta http-equiv="expires"
 content="Fri, 04 Apr 2014 23:59:59 GMT" />
</head>
<body>
</body>
</html>
```

## HTML5 Layout

HTML5 introduces a new set of elements that allow you to divide up the parts of a page. The names of 

these elements indicate the kind of content you will find in them. They are still subject to change, 

but that has not stopped many web page authors using them already.

* The ```<header>``` and ```<footer>``` elements can be used for:

  * The main header or footer that appears at the top or bottom of every page on the site.
  * A header or footer for anindividual ```<article>``` or ```<section>``` within the page.

* The ```<nav>``` element is used to contain the major navigational blocks on the site such as the primary 

site navigation.

* The ```<article>``` element acts as a container for any section of a page that could stand alone and 

potentially be syndicated. This could be an individual article or blog entry, a comment or forum post, 

or any other independent piece of content.

* The ```<aside>``` element has two purposes, depending on whether it is inside an ```<article>```

element or not.

When the ```<aside>``` element is used inside an <article> element, it should contain information that 

is related to the article but not essential to its overall meaning. For example, a pullquote or 

glossary 

might be considered as an aside to the article it relates to.

When the ```<aside>``` element is used outside of an ```<article>``` element, it acts as a container for content 

that is related to the entire page. For example, it might contain links to other sections of the site 

a list of recent posts, a search box, or recent tweets by the author.

* The ```<section>``` element groups related content together, and typically each section would have 

its own heading.

*  The ```<hgroup>``` element is to group together a set of one or more <h1> through <h6> elements so 

that they are treated as one single heading.

* ```<figure>```  It can be used to contain any content that is referenced from the main flow of an 

article (not just images).

* the ```<div>``` element will remain an important way to group together related elements, because you 

should not be using these new elements that you have just met for purposes other than those explicitly 

stated.


## Process & Design


### Who is the Site For?

Every website should be designed for the target audience—not just for yourself or the site owner. It 

is therefore very important tounderstand who your target audience is.



#### Target Audience: individuals

* What is the age range of your target audience?

* Will your site appeal to more women or men? What is the mix?

* Which country do your visitors live in?

* Do they live in urban or rural areas?

* What is the average income of visitors?

* What level of education do they have?

* What is their marital or family status?

* What is their occupation?

* How many hours do they work per week?

* How often do they use the web?

* What kind of device do they use to access the web?

#### Target Audience: Companies

* What is the size of the company or relevant department?

* What is the position of people in the company who visit your site?

* Will visitors be using the site for themselves or for someone else?

* How large is the budget they control?



# JavaScript

## The ABC of Programming

### [ A ] What is a script and how do I create one?

* **A script is a series of instructions** 

A script is a series of instructions that a computer can follow to 

achieve a goal.

You could compare scripts to any of the following: 

  * RECIPES
  
  Some scripts are simple and only deal with one individual scenario,

like a simple recipe for a basic dish. Other scripts can perform many 

tasks, like a recipe for a complicated three-course meal. 

  * HANDBOOKS 

  Large companies often provide handbooks for new employees that 

  contain procedures to follow in certain situations.

  * MANUALS

   Mechanics often refer to car repair manuals when servicing models 
  
  they are not familiar with. These manuals contain a series of 
    
  tests 
  
  to check the key functions of the car are working, along with 
  
  details of how to fix any issues that arise.


* **Writing a script **

To write a script, you need to first state your goal and then list the

tasks that need to be completed in order to achieve it. 
 
* ** Defining a goal & dsigning the script **

Consider how you might approach a different type of script.

* ** Sketching out the tasks in a flowchart**
Often scripts will need to perform different tasks in different 

situations.

You can use flowcharts to work out how the tasks fit together.

The flowcharts show the paths between each step. 

### [B] How do computers fit in with  the world around them? 

* **Computers create models of the world using data**

* **OBJECTS & PROPERTIES **

Each object can have its own:

  - Properties

  - Events

  - Methods 

Each property has a name and a value, and each of these name/value 

pairs tells you something about each individual instance of the object


* **EVENTS**

Programmers choose which events they respond to. When a specific 

event happens, that event can be used to trigger a specific section 

of the code. 

* **METHODS**

Methods represent things people need to do with objects. They can

retrieve or update the values of an object's properties. 

* **PUTTING IT ALL TOGETHER** 

Computers use data to create models of things in the real world.

The events, methods, and properties of an object all relate to each 

other:

Events can trigger methods, and methods can retrieve or update an

object's properties. 

* **WEB BROWSERS ARE PROGRAMS BUILT USING OBJECTS **


* **THE DOCUMENT OBJECT REPRESENTS AN HTML PAGE**

Using the document object, you can access and change what content

users see on the page and respond to how they interact with it.

### [C] How do I write a script for a web page? 

* **HOW HTML, CSS, & JAVASCRIPT FIT TOGETHER **

Before diving into the JavaScript language, you need to know how it 

will fit together with the HTML and CSS in your web pages. 

Web developers usually talk about three languages that are used to 

create web pages:

HTML, CSS, and JavaScript. 

Where possible, aim to keep the hree languages in separate files, 

with the HTML page linking to CSS and JavaScript files

Each language forms a separate layer with a different purpose.

Each layer, from left to right. builds on the previous one.

* **PROGRESSIVE ENHANCEMENT**

These three layers form the basis of a popular approach to building 

web pages called progressive enhancement.

As more and more web-enabled devices come onto the market, this 

concept is becoming more widely adopted. 

It's not just screen sizes that are varied - connection speeds and

capabilities of each device can also differ. 

some people browse with JavaScript turned off, so you need to make 

sure that the page still works for them. 

* **CREATING A BASIC JAVASCRIPT **

JavaScript is written in plain text, just like HTML and CSS, so you 

do not need any new tools to write a script. This example adds a 

greeting into an HTML page. The greeting changes depending on the 

time of day. 

* **LINKING TO A JAVASCRIPT FILE FROM AN HTML PAGE**

When you want to use JavaScript with a web page, you use the HTML

```<script>``` element to tell the browser it is coming across a 

script. Its s re attribute tells people where the JavaScript file is 

stored.

* **THE SOURCE CODE IS NOT AMENDED**


* **PLACING THE SCRIPT IN THE PAGE**