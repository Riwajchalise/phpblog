---
title: Introdution to HTML  
keywords: documentation PHP, HTML, Introduction to HTML, HTML tutorial
last_updated: July 3, 2016
tags: 
summary: "HTML one of the major prerequisite you need to have in order to understand php."
sidebar: mydoc_sidebar
permalink: mydoc_introduction_to_HTML.html
folder: mydoc
---

## What is HTML? 
* HTML stands for Hypertext Markup Language. 
* HTML is a the markup language designed for creating the webpage.
* HTML describes the structure of the web page.
* HTML elements are represented by tags.
* Browser uses HTML tags to render HTML content.

{% include note.html content="The file extension for a HTML file is .html" %}

## A Basic HTML Document?

{% highlight html %}
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>Heading</h1>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. </p>

</body>
</html>
{% endhighlight %}


### Understanding the tags

* The ```<!DOCTYPE html>``` declaration defines this document to be HTML5
* The ```<html>``` element is the root element of an HTML page
* The ```<head>``` element contains meta information about the document
* The ```<title>``` element specifies a title for the document
* The ```<body>``` element contains the visible page content
* The ```<h1>``` element defines a large heading
* The ```<p>``` element defines a paragraph

{% include important.html content="Some of the important in html are ```<table>```, ```<form>```, ```<img>``` etc." %}

{% include callout.html content="
If you want to know more about HTML you can check the [HTML_tutorial](https://www.w3schools.com/html/default.asp) by w3 school.
" type="primary" %} 


