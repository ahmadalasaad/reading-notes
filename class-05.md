# IMAGES

There are many reasons why you might want to add an image to a web page: you might want to include a logo, photograph, illustration, 

diagram, or chart.

* **Adding Images**

```<img>```

To add an image into the page you need to use an ```<img>``` element. This is an empty 

element (which means there is no closing tag). It must carry the following two attributes:

src

This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your 

own site. (Here you can see that the images are in a child folder called images — relative URLs were covered on pages 83-84). 

alt

This provides a text description of the image which describes the image if you cannot see it.

title

You can also use the titleattribute with the ```<img>``` element to provide additional information about the image. Most browsers 

will display the content of this attribute in a tootip when the user hovers over the image.

```
<img src="images/quokka.jpg" alt="A family of 
 quokka" title="The quokka is an Australian 
 marsupial that is similar in size to the 
 domestic cat." />

```

* **Height & Width of Images**

height

This specifies the height of the image in pixels.

width

This specifies the width of the image in pixels.

```
<img src="images/quokka.jpg" alt="A family of 
 quokka" width="600" height="450" />

 ```


 # Color

 Color can really bring your pages to life.

 * **Foreground Color**
color

 The color property allows you to specify the color of text inside an element. 
 
 You can specify any color in CSS in one of three ways:

rgb values

These express colors in terms of how much red, green and blue are used to make it up. For 

example: rgb(100,100,90)

 hex codes

These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign.
 
 For example: #ee3e80

color names

There are 147 predefined color names that are recognized by browsers. For example: DarkCyan

* **Background Color**

background-color

CSS treats each HTML element as if it appears in a box, and the background-color property 

sets the color of the background for that box.

You can specify your choice of background color in the same three ways you can specify foreground colors: 

RGB values, hex codes, and color names (covered on the next page).

If you do not specify a background color, then the background is transparent. 

By default, most browser windows have a white background, but browser users can set a background color for 

their windows, so if you want to be sure that the background is white you can use the background-color property on the ```<body>```

 element.

 # TEXT 

* **Specifying Typefaces**

font-family

The font-family property allows you to specify the typeface that should be used for any text inside the element(s) to 

which a CSS rule applies.

The value of this property is the name of the typeface you want to use. 

The people who are visiting your site need the typeface you have specified installed on their computer in order for it to be displayed. 

You can specify a list of fonts separated by commas so that, if the user does not have your first choice of typeface installed, 

the browser can try to use an alternative font from the list.

It is also common to end with a generic font name for that type 

of font.

If a font name is made up of more than one word, it should be put in double quotes.

Designers suggest pages usually look better if they use no more than three typefaces on a page.

```
<!DOCTYPE html>
<html>
<head>
 <title>Font Family</title>
 <style type="text/css">
 body {
 font-family: Georgia, Times, serif;}
 h1, h2 {
 font-family: Arial, Verdana, sans-serif;}
 .credits {
 font-family: "Courier New", Courier, 
 monospace;}
 </style>
</head>
<body>
 <h1>Briards</h1>
 <p class="credits">by Ivy Duckett</p>
 <p class="intro">The <a class="breed" 
 href="http://en.wikipedia.org/wiki/
 Briard">briard</a>, or berger de brie, is 
 a large breed of dog traditionally used as 
 a herder and guardian of sheep...</p>
</body>
</html>
```

* In addition to the CSS properties covered in other chapters which work with the contents of all elements, 

there are several others that are specifically used to control the appearance of lists, tables, and forms.

* List markers can be given different appearances using the list-style-type and list-style image properties.

* Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and 

make them more consistent. 

* Forms are easier to use if the form controls are vertically aligned using CSS.

* Forms benefit from styles that make them feel more interactive.

# JPEG vs PNG vs GIF

* JPEG is a lossy compression specification that takes advantage of human perception.

* PNG is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are 

introduced in the image.

* GIF is also a lossless image format that uses LZW compression algorithm.