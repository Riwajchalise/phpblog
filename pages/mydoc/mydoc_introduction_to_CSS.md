<!-- ---
title: Introdution to CSS  
keywords: documentation theme, jekyll, technical writers, help authoring tools, hat replacements
last_updated: July 3, 2016
tags: 
summary: "CSS is another major prerequisite you need to have in order to understand php."
sidebar: mydoc_sidebar
permalink: mydoc_introduction_to_CSS.html
folder: mydoc
---

## What is a CSS?
* CSS stands for Cascading Style Sheets
* CSS describes how HTML elements are to be displayed on screen, paper, or in other media
* External stylesheets are stored in CSS files

{% include note.html content="The file extension for an external CSS file is .CSS" %}

## Three basic ways of implementing CSS

### 1. Inline CSS
The inline CSS is written to uniquly style a single element.

Inline styles are defined within the "style" attribute of the relevant element:

#### Example of inline CSS
{% highlight html %}
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
{% endhighlight %}

[DEMO](https://codepen.io/riwajchalise/pen/QWWBjYm)

### 2. Internal CSS
The internal style is defined inside the ```<style>``` element, inside the head section.

#### Exmaple of Internal CSS
{% highlight html %}
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
{% endhighlight %}

[DEMO](https://codepen.io/riwajchalise/pen/QWWBjPr)

### 3. External CSS
External styles are defined within the  ```<link>``` element, inside the ```<head>``` section of an HTML page:

#### Example of External CSS
{% highlight html %}
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
{% endhighlight %}

Here is how the "mystyle.css" file looks like:

{% highlight css %}
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
{% endhighlight %}

[DEMO](https://codepen.io/riwajchalise/pen/ZEEjQEP)

{% include important.html content="A CSS file should not contain html tags" %}

{% include callout.html content="
If you want to know more about CSS you can check the [CSS_tutorial](https://www.w3schools.com/css/default.asp) by w3 school.
" type="primary" %} 

{% include links.html %} -->
