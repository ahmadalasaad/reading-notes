# Understanding the problem domain is the hardest part of programming 

What is the hardest thing about writing code?

There are many common answers to this question:

* Learning a new technology
* Naming things
* Testing your code
* Debugging
* Fixing bugs
* Making software maintainable


# Object Literals

Objects group together a set of variables and functions to create a model 

of a something you would recognize from the real world. In an object, 

variables and functions take on new names.

* **CREATING· OBJECTS USING LITERAL NOTATION**

This example starts by creating an object using literal notation. 

This object is called hotel which represents a hotel called Quay 

with 40 rooms (25 of which have been booked). 

Next, the content of the page is updated with data from this 

object. It shows the name of the hotel by accessing the object's 

name property and the number of vacant rooms using the 

checkAvailability() method. 

To access a property of this object, the object name is 

followed by a dot (the period symbol) and the name of the 

property that you want. 

Similarly, to use the method, you can use the object name 

followed by the method name. 

hotel.checkAvailability() If the method needs parameters, you can supply them in the parentheses (just like you can pass arguments to a function)

```
var hote l = { 
name: 'Quay', 
rooms: 40, 
booked : 25, 
checkAvailability: function() { 
return this.rooms - this.booked; 
} 
} ; 
JAVASCRIPT 
var el Name = document .getElementByld('hotelName'); 
elName.textContent =hotel .name; 
var elRooms = document.getElementByid{'rooms'); 
elRooms.textContent = hotel .checkAvailability(); 

```

# Document Object Model

The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how 

JavaScript can access and update the contents of a web page while it is in the browser window.

* **WORKING WITH THE DOM TREE**

Accessing and updating the DOM tree involves two steps:


1: Locate the node that represents the element you want to work with. 

2: Use its text content, child elements, and attributes

* **ACCESSING ELEMENTS**

DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes. 

GROUPS OF ELEMENT NODES 

If a method can return more than one node, it will always return a Nodelist, which is a collection of 

nodes (even if it only finds one matching element). You then need to select the element you want from 

this list using an index number (which means the numbering starts at 0 like the items in an array). 

For example, several elements can have the same tag name, so ```get El ementsByTagName () ``` will always 

return a Nodel i st.

FASTEST ROUTE

Finding the quickest way to access an element within your web page will make the page seem 

faster and/or more responsive. This usually means evaluating the minimum number of nodes on the 

way to the element you want to work with. For example, getEl ementByld () will quickly return one 

element (because no two elements on the same page should have the same value for an id attribute), 

but it can only be used when the element you want to access has an id attribute. 

* METHODS THAT RETURN A SINGLE ELEMENT NODE:

```getElementByld( 'id')```

Selects an individual element given the value of its i d attribute . 

The HTML must have an id attribute in order for it to be selectable. 

``` querySel ector( 'css selector')``` 

Uses CSS selector syntax that would select one or more elements . 

This method returns only the first of the matching elements.

METHODS THAT RETURN ONE OR MORE ELEMENTS (AS A NODELIST):

getEl ementsByClassName('class') 

Selects one or more elements given the value of their cl ass attribute. 
The HTML must have a cl ass attribute for it to be selectable. 
This method is faster than query SelectorAll () . 

getEl ementsByTagName('tagName') 

Selects all elements on the page with the specified tag name. 

This method is faster than query SelectorAll () . 

querySelectorAll ('css selector') 

Uses CSS selector syntax to select one or more elements and returns all 

of those that match. 

