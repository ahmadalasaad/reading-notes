# IMAGES

* CONTROLLING SIZE OF IMAGES

You can control the size of an 
image using the width and 
height properties in CSS, just 
like you can for any other box.

```
<img src="images/magnolia-large.jpg"
 class="large" alt="Magnolia" /> 
<img src="images/magnolia-medium.jpg"
 class="medium" alt="Magnolia" /> 
<img src="images/magnolia-small.jpg"
 class="small" alt="Magnolia" />

```
```
<img src="images/magnolia-large.jpg"
 class="large" alt="Magnolia" /> 
<img src="images/magnolia-medium.jpg"
 class="medium" alt="Magnolia" /> 
<img src="images/magnolia-small.jpg"
 class="small" alt="Magnolia" />

```

* AligNing images


```
<p><img src="images/magnolia-medium.jpg" 
 alt="Magnolia" class="align-left medium" />
 <b><i>Magnolia</i></b> is a large genus that 
 contains over 200 flowering plant species...</p>
<p><img src="images/magnolia-medium.jpg" 
 alt="Magnolia" class="align-right medium" />
Some magnolias, such as <i>Magnolia stellata</i>
 and <i>Magnolia soulangeana</i>, flower quite 
 early in the spring before the leaves open...</p>

```

```
img.align-left {
float: left;
margin-right: 10px;}
img.align-right {
float: right;
margin-left: 10px;}
img.medium {
width: 250px;
height: 250px;}

```

* Centering images

```
<p><img src="images/magnolia-medium.jpg" 
 alt="Magnolia" class="align-center medium" />
 <b><i>Magnolia</i></b> is a large genus that 
 contains over 200 flowering plant species. It 
 is named after French botanist Pierre Magnol and, 
 having evolved before bees appeared, the 
 flowers were developed to encourage pollination 
 by beetle.</p>

```

```
img.align-center { 
display: block; 
margin: 0px auto;} 
img.medium { 
width: 250px; 
height: 250px;}

```

# Practical Information

**Search Engine Optimization**

SEO is a huge topic and several books have been written on the subject. 
The following pages will help you understand the key concepts so you can 
improve your website's visibility on search engines.

* The Basics

Search engine optimization (or 
SEO) is the practice of trying 
to help your site appear nearer 
the top of search engine results 
when people look for the topics 
that your website covers.

At the heart of SEO is the idea of 
working out which terms people 
are likely to enter into a search 
engine to find your site and then 
using these terms in the right 
places on your site to increase 
the chances that search engines 
will show a link to your site in 
their results.

In order to determine who comes 
first in the search results, search 
engines do not only look at what 
appears on your site. They also 
consider how many sites link 
to you (and how relevant those 
links are). For this reason, SEO 
is often split into two areas: 
on-page techniques and off-page 
techniques.

* On-Page Techniques

On-page techniques are the 
methods you can use on your 
web pages to improve their 
rating in search engines.
The main component of this is 
looking at keywords that people 
are likely to enter into a search 
engine if they wanted to find 
your site, and then including 
these in the text and HTML code 
for your site in order to help the 
search engines know that your 
site covers these topics.

Search engines rely very heavily 
on the text that is in your pages 
so it is important that the terms 
people are going to search for 
are in text. There are seven 
essential places where you want 
your keywords to appear.

Ensuring that any images have 
appropriate text in the value of 
their alt attribute also helps 
search engines understand the 
content of images.

* Off-Page Techniques

Getting other sites to link to you 
is just as important as on-page 
techniques. Search engines help 
determine how to rank your 
site by looking at the number of 
other sites that link to yours.
They are particularly interested 
in sites whose content is related 
to yours. For example, if you 
were running a website that 
sold fish bait, then a link from 
a hairdresser is not likely to be 
considered as relevant as one 
from an angling community.

Search engines also look at the 
words between the opening 
`<a>` tag and closing `</a>` tag 
in the link. If the text in the link 
contains keywords (rather than 
just click here or your website 
address) it may be considered 
more relevant.

The words that appear in links to 
your site should also appear in 
the text of the page that the site 
links to.