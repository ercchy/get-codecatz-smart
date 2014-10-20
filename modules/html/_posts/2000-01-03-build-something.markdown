---
title: Build Something
published: true
---

# Get started: folder structure

All the files for your site should be stored within the same folder.

This includes:

* HTML Files 

* CSS Files 

* Images 

* Script files 

* Anything else that will appear on your site 


Note: File names should not include spaces or special characters. File names ARE case sensitive.

![Folder Structure]({{site.baseurl}}/img/codecatz/folderstructure1.png)

###ANATOMY OF A WEBSITE

Your Content
+ HTML: Structure
+ CSS: Presentation
= Your Website

A website is a way to present your content to the world, using HTML and CSS to present that content & make it look good.

####Concrete example
* A **paragraph** is your content  
Putting your content into an HTML tag to make it look like a paragraph is Structure  
{% highlight yaml %}
<p>A paragraph is your content</p>
{% endhighlight %}

* **Element** 
Is an individual component of HTML. Examples of elements are: 
Paragraph, heading, table, list, div, link, image, etc.  

* **Tag**  
Marks the beginning & end of an element. 
There are Opening tag and Closing Tag, and they contain characters that indicate the tags purpose

{% highlight yaml %}
<tagname>Stuff in the middle</tagname>
{% endhighlight %}

{% highlight yaml %}
<p> This is a sample paragraph.</p>
{% endhighlight %}

![Tag Breakdown]({{site.baseurl}}/img/codecatz/tagbreakdown.png)

* **Container Element**  
An element that can contain other elements or content. For example a paragraph

{% highlight yaml %} <p>{% endhighlight %} contains text

* **Stand Alone Element**  
An element that cannot contain anything else

{% highlight yaml %}
<br/>
<img/> 
{% endhighlight %}

* **Attribute**  
Provides additional information about the HTML element. We know Class, ID, 
language, style, identity, source. They are placed inside an opening tag, 
before the right angle bracket.

* **Value**  
Value is the value assigned to a given attribute. They must be contained inside quotation marks.
{% highlight yaml %}
<div id="copyright">CC-BY-SA</div>
<img src="my_picture.jpg" /> 
<a href="http://codecatz.com">CodeCatz</a> 
{% endhighlight %}

###DOCTYPE

The ﬁrst thing on an HTML page is the doctype, which tells the browser which version of the markup language the page is using.

{% highlight yaml %}
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML
  4.01 Transitional//EN" "http://
  www.w3.org/TR/html4/loose.dtd">
{% endhighlight %}

{% highlight yaml %}
<!DOCTYPE html>
{% endhighlight %}

The doctype is case-insensitive. 
DOCtype, doctype, DocType and DoCtYpe are all valid.

###HTML TAG
After ```<doctype>```, the page content must be contained between ```<html>``` tags.
{% highlight yaml %}
<!DOCTYPE html>
<html>

</html>
{% endhighlight %}

###HEAD AND BODY TAGS

**Head**: The head contains the title of the page & meta information about the page. 
Meta information is not visible to the user, but has many purposes 
One of which is to tell search engines about your page, who created it, and a 
description.

**Body**: The body contains the actual content of the page. 
Everything that is contained in the body is visible to the user.

{% highlight yaml %}
<!DOCTYPE html>
<html>
   <head>
	<title>Title of the page </title>
   </head>
   <body>
	The page content here.
   </body>
</html>
{% endhighlight %}

***
##CAT Action!
Let's get our web page set up with a doctype, head, title and body.
Later we'll add some content to it!
***

###NESTING

All elements "nest" inside one another. 
Nesting is what happens when you put other containing tags inside other 
containing tags. For example, you would put the ```<p>``` inside 
of the ```<body>``` tags. The ```<p>``` is now nested inside the ```<body>```.
Whichever element OPENS first CLOSES last.

![Nesting dolls]({{site.baseurl}}/img/codecatz/nestingdolls.jpg)

##### Example:

Elements are 'nested' inside the ```<body>``` tag.

{% highlight yaml %}
<body>
   <p>A paragraph inside the body tag</p>
</body>
{% endhighlight %}

Paragraphs 'nested' inside list items.

{% highlight yaml %}
<ul>
   <li>
	  <p>A paragraph inside a list item</p>
   </li>
</ul>
{% endhighlight %}

###ELEMENT: PARAGRAPH
White space is only for humans!

{% highlight yaml %}
<p>Paragraph 1</p>
<p>Paragraph 2</p>
<p>Paragraph 3</p>
{% endhighlight %}

{% highlight yaml %}
<p>Paragraph 1</p> <p>Paragraph 2</p>  <p>Paragraph 3</p>
{% endhighlight %}

{% highlight yaml %}
<p>Paragraph 1</p> 
  
  
<p>Paragraph 2</p>  
<p>Paragraph 3</p>
{% endhighlight %}
This will all render the same way!

<p>Paragraph 1</p>
<p>Paragraph 2</p>
<p>Paragraph 3</p>

####Paragraphs
Paragraphs allow you to format your content in a readable fashion. You can edit how paragraphs are displayed with CSS

```
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque dignissim, metus sed vehicula porttitor, orci dui lacinia tellus, id semper diam lorem non mauris. Proin sapien turpis, mattis ut nisi quis, blandit imperdiet odio. Maecenas efficitur imperdiet fringilla. Mauris vestibulum sem ut tortor malesuada, in mollis quam placerat. Mauris maximus mi erat, ut ultrices nibh aliquam sed. Cras dapibus sagittis diam, vel venenatis risus hendrerit eget. Etiam sed diam pulvinar, fermentum mi vitae, maximus justo. Nulla rhoncus neque ac molestie imperdiet.

Phasellus molestie suscipit mi sit amet convallis. Maecenas vulputate sapien nec turpis cursus fringilla. Vivamus tempus lacinia tortor, sit amet accumsan arcu volutpat fermentum. Praesent sed placerat nisl. Curabitur eu vulputate augue. Nam vulputate libero ac vestibulum feugiat. Donec blandit vel ante eu molestie. Suspendisse sit amet elit quis nulla dapibus blandit ut id ex.

Quisque a tellus sed dolor cursus fermentum. Etiam ultricies sem sit amet ultricies molestie. Cras neque felis, ornare nec augue sit amet, tincidunt scelerisque eros. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Vestibulum efficitur elit quam. Aliquam luctus, mauris at hendrerit gravida, metus massa vehicula nisi, sit amet feugiat est est non libero. Integer felis dolor, luctus tempus mattis sit amet, pellentesque et neque. Phasellus at lobortis nisl, a maximus tellus. Suspendisse vitae porttitor erat. Quisque ipsum nulla, scelerisque eu volutpat eu, viverra in libero.

```

###ELEMENT: HEADING
Heading number indicates hierarchy, not size. Think: Outlines from high school papers

{% highlight yaml %}
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
{% endhighlight %}

####Example:
![Headings]({{site.baseurl}}/img/codecatz/example-headings.png)

###FORMATTED TEXT
```em``` and ```strong``` are meant to indicate meaning through style. If you want to have italicized for appearance and not to communicate meaning, you should use CSS.

<p>
  Here is a paragraph with <em>Emphasized</em> text and <strong>Important</strong> text.
</p>
{% highlight yaml %}
<p>
  Here is a paragraph with <em>Emphasized</em> text and <strong>Important</strong> text.
</p>
{% endhighlight %}

***
## CAT Action
Let's add some content to our site!
Add one of each level of heading with 1-2 short paragraphs of text below each heading.
Italic and bold some text within a few paragraphs.
***

###ELEMENT: LINK

Links have three components:

* Tag: <a></a> 
* Href attribute: "http://codecatz.org" 
* Title attribute: "CodeCatz" 

{% highlight yaml %}
<a href="http://codecatz.com" title="CodeCatz">CodeCatz</a>
{% endhighlight %}

The ```<a>``` tag surrounds text or images to turn them into links.

###LINK ATTRIBUTES

Links can have attributes that tell the link to do different actions like open in a new tab, or launch your e-mail program.

Link opens in a new window/tab with target="_blank"
{% highlight yaml %}
<a href="home.html" target="_blank">Link Text</a>
{% endhighlight %}

Link opens mail program by inserting mailto: directly before the email address.
{% highlight yaml %}
<a href="mailto:info@girldevelopit.com">E-mail us!</a>
{% endhighlight %}

###RELATIVE VS. ABSOLUTE PATHS FOR LINKS & IMAGES

* **Relative**  
  * Relative paths change depending upon the page the link is on.   
    * Links within the same directory need no path information. ```"filename.jpg"```   
    * Subdirectories are listed without preceding slashes. ```"images/filename.jpg"```   
    
* **Absolute**
  * Absolute paths refer to a specific location of a file, including the domain. ```"http://www.girldevelopit.com/chapters/detroit"```
  * Typically used when pointing to a link that is not within your own domain.
  

***
##CAT Action

Let's add links to our site!
Add links that open in the same window, a new window and link to an e-mail address.

***

###ELEMENT: IMAGE

Images have three components

* Tag: ```<img/>```
* Src attribute: ```"http://codecatz.org/assets/logo.png"```
* Alt attribute: "CodeCatz Logo"

{% highlight yaml %}
<img src ="http://codecatz/assets/logo.png" alt = "CodeCatz Logo"/>
{% endhighlight %}

![CodeCatz Logo]({{site.baseurl}}/img/codecatz/logo.png)

Notice: This tag is our first example of a stand-alone or "self-closing" element.

###ELEMENT: LINE BREAK
This is how you break a line:

{% highlight yaml %}
<p>
  Imagine there's no Heaven <br/>
  It's easy if you try <br/>
  No hell below us  <br/>
  Above us only sky
</p>
{% endhighlight %}


***
##CAT Action

Let's add some images and line breaks to our page.
We can even turn our images into links!

***

###ELEMENT: UNORDERED AND ORDERED LISTS

{% highlight yaml %}
<ul>
	<li>List Item</li>
	<li>AnotherList Item</li>
</ul>
{% endhighlight %}
<ul>
	<li>List Item</li>
	<li>AnotherList Item</li>
</ul>

{% highlight yaml %}
<ol>
	<li>List Item</li>
	<li>AnotherList Item</li>
</ol>
{% endhighlight %}
<ol>
	<li>List Item</li>
	<li>AnotherList Item</li>
</ol>

####Examples:
Lists can be used to organize any list of items.

![List Examples]({{site.baseurl}}/img/codecatz/example-lists.png)

***
##CAT Action

Let's add one of each ordered and unordered lists to our page.
We can make a list of links or even a list of images!

***

###COMMENTS

You can add comments to your code that will not be seen by the browser, but only visible when viewing the code.

{% highlight yaml %}
<!-- Comment goes here -->
{% endhighlight %}

Comments can be used to organize your code into sections so you 
(or someone else) can easily understand your code. It can also be used to 
'comment out' large chunks of code to hide it from the browser.

{% highlight yaml %}
<!-- Beginning of header -->
   <div id="header">Header Content </div>
<!-- End of header -->

<!--   
  <ol>
    <li>List Item</li>
    <li>Another List Item</li>
  </ol> 
--> 
{% endhighlight %}

###TABLES

Tables are a way to represent complex information in a grid format.
Tables are made up of rows and columns.

{% highlight yaml %}
<table>
  <tr> 
    <th>Head</th>
    <th>Head</th>
  </tr>
  <tr> 
    <td>Data</td>
    <td>Data</td>
  </tr>
</table>
{% endhighlight %}
<table>
  <tr> 
    <th>Head</th>
    <th>Head</th>
  </tr>
  <tr> 
    <td>Data</td>
    <td>Data</td>
  </tr>
</table>

####Examples:

Tables can be styled with CSS to add zebra striping or to highlight important rows/columns.

![Tables]({{site.baseurl}}/img/codecatz/example-tables.png)

###CHARACTER CODES
There are character codes for many different characters in many different languages

* Delta: ```&delta;``` δ  
* Copyright symbol: ```&copy;``` © 
* Grave: ```&grave;``` ` 
* An grave a: ```&agrave;``` à 

A full list is available at [http://www.ascii.cl/htmlcodes.htm](http://www.ascii.cl/htmlcodes.htm)

