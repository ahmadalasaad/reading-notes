# css

## what is css ?

CSS (Cascading Style Sheets) allows you to create great-looking web 

pages, but how does it work under the hood? This article explains 

what CSS is, with a simple syntax example, and also covers some key 

terms about the language.

## There are three ways of inserting a style sheet:
* **External CSS**

With an external style sheet, you can change the look of an entire 

website by changing just one file!

Each HTML page must include a reference to the external style sheet 

file inside the <link> element, inside the head section.

< head >

< link rel="stylesheet" href="mystyle.css">

< /head >

* **Internal CSS**

< head >

< style >

body {

  background-color: linen;

}

h1 {

  color: maroon;

  margin-left: 40px;

}
< /style >

< /head >

* **Inline CSS**

< body >

< h1 style="color:blue;text-align:center;">This is a heading< /h1 >

< p style="color:red;" > This is a paragraph.< /p >

< /body >