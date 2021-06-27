# Domain Modeling


Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

Here's some tips to follow when building your own domain models.

When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
Model its attributes with a constructor function that defines and initializes properties.
Model its behaviors with small methods that focus on doing one job well.
Create instances using the new keyword followed by a call to a constructor function.
Store the newly created object in a variable so you can access its properties and methods from outside.
Use the this variable within methods so you can access the object's properties and methods from inside.


# Tables

A table represents information in a grid format. 
Examples of tables include financial reports, TV 
schedules, and sports results.

* **Basic Table Structure**

```<table>```

The ```<table>``` element is used 
to create a table. The contents 
of the table are written out row 
by row.

```<tr>```

You indicate the start of each 
row using the opening ```<tr>``` tag. 
(The tr stands for table row.) 
It is followed by one or more 
```<td>``` elements (one for each cell 
in that row). 
At the end of the row you use a 
closing ```</tr>`` tag.

```<td>```
Each cell of a table is 
represented using a ```<td>```
element. (The td stands for 
table data.)
At the end of each cell you use a 
closing ```</td>``` tag

```
<table>
 <tr>
 <td>15</td>
 <td>15</td>
 <td>30</td>
 </tr>
 <tr>
 <td>45</td>
 <td>60</td>
 <td>45</td>
 </tr>
 <tr>
 <td>60</td>
 <td>90</td>
 <td>90</td>
 </tr>
</table>

```

* **Table Headings**

```<th>```

The ```<th>``` element is used just 
like the ```<td>``` element but its 
purpose is to represent the 
heading for either a column or 
a row. (The th stands for table 
heading.) 

Even if a cell has no content, 
you should still use a ```<td>``` or 
```<th>``` element to represent 
the presence of an empty cell 
otherwise the table will not 
render correctly. (The first cell 
in the first row of this example 
shows an empty cell.)

Using ```<th>``` elements for 
headings helps people who 
use screen readers, improves 
the ability for search engines 
to index your pages, and also 
enables you to control the 
appearance of tables better 
when you start to use CSS.

You can use the scope attribute 
on the ```<th>``` element to indicate 
whether it is a heading for a 
column or a row. It can take the 
values: row to indicate a heading 
for a row or col to indicate a 
heading for a column.

```
<table>
 <tr>
 <th></th>
 <th scope="col">Saturday</th>
 <th scope="col">Sunday</th>
 </tr>
 <tr>
 <th scope="row">Tickets sold:</th>
 <td>120</td>
 <td>135</td>
 </tr>
 <tr>
 <th scope="row">Total sales:</th>
 <td>$600</td>
 <td>$675</td>
 </tr>
</table>

```

* **Spanning ColumnS**

```
<table>
 <tr>
 <th></th>
 <th>9am</th>
 <th>10am</th>
 <th>11am</th>
 <th>12am</th>
 </tr>
 <tr>
 <th>Monday</th>
 <td colspan="2">Geography</td>
 <td>Math</td>
 <td>Art</td>
 </tr>
 <tr>
 <th>Tuesday</th>
 <td colspan="3">Gym</td>
 <td>Home Ec</td>
 </tr>
</table>

```

* **Spanning Rows**
```
<table>
 <tr>
 <th></th>
 <th>ABC</th>
 <th>BBC</th>
 <th>CNN</th>
 </tr>
 <tr>
 <th>6pm - 7pm</th>
 <td rowspan="2">Movie</td>
 <td>Comedy</td>
 <td>News</td>
 </tr>
 <tr>
 <th>7pm - 8pm</th>
 <td>Sport</td>
 <td>Current Affairs</td>
 </tr>
</table>

```
* **Long Tables**
```

<table>
 <thead>
 <tr>
 <th>Date</th>
 <th>Income</th>
 <th>Expenditure</th>
 </tr>
 </thead>
 <tbody>
 <tr>
 <th>1st January</th>
 <td>250</td>
 <td>36</td>
 </tr>
 <tr>
 <th>2nd January</th>
 <td>285</td>
 <td>48</td>
 </tr>
 <!-- additional rows as above -->
 <tr>
 <th>31st January</th>
 <td>129</td>
 <td>64</td>
 </tr>
 </tbody>
 <tfoot>
 <tr>
 <td></td>
 <td>7824</td>
 <td>1241</td>
 </tr>
 </tfoot>
</table>

```

# Functions, Methods, and Objects

 Objects group together a set of variables and functions to create a model 
of a something you would recognize from the real world. In an object, 
variables and functions take on new names. 

* **CREATING OBJECTS USING CONSTRUCTOR SYNTAX**

```
var hotel = new Object(); 
hotel.name= 'Park'; 
hotel.rooms = 120; 
hotel .booked = 77; 
hotel .checkAvailability = function() 
return this.rooms - this.booked; 
} ; 
JAVASCRIPT 
var elName = document.getElementByid('hotelName'); 
elName.textContent = hotel . name; 
var elRooms = document .getElementByid('rooms'); 
elRooms.textContent = hotel .checkAvailability(};

```

* **CREATE & ACCESS OBJECTS CONSTRUCTOR NOTATION**

```

function Hotel (name, rooms, booked) { 
this.name = name; 
this.rooms = rooms; 
this.booked = booked; 
this.checkAvailability = function() 
return this.rooms - this.booked; 
} ; 
var quayHotel 
var parkHotel 
new Hotel('Quay', 40, 25); 
new Hotel( ' Park', 120, 77); 
var details!= quayHotel .name + ' rooms : '; 
detailsl += quayHotel.checkAvailability(); 
var elHotell = docurnent.getElementByid('hotell'); 
elHotell.textContent =details!; 
var details2 = parkHotel .name+ ' rooms: '; 
detai ls2 += parkHotel.checkAvailability(); 
var e1Hotel2 = document.getEl ementByid('hotel2'); 
elHotel2.textContent = details2; 

```

* **ADDING AND REMOVING PROPERTIES**

```
var hotel = { 
name : 'Park' , 
rooms : 120, 
booked : 77. 
} ; 
hotel .gym = t rue; 
hotel .pool = fal se; 
delete hotel .booked; 
var elName = document .getEl ementByld('hotelName '); 
elName.textContent = hotel . name; 
var el Pool = document .getElementByid ('pool ') ; 
elPool.cl assName = ' Pool: ' + hotel. pool ; 
var elGym = document .getEl ementByld('gym' }; 
elGym.className = 'Gym: ' + hotel .gym; 

```

