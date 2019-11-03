---
title: HTML Forms 
keywords: Forms, Forms in html, Form design, HTML forms
last_updated: November 1, 2019
tags: 
summary: "This post will give you the brief introduction about HTML forms. The resources available here is just enough to understand this course. "
sidebar: mydoc_sidebar
permalink: mydoc_forms.html
folder: mydoc
---

## The ```<form>``` Tag

The html form is defined by ```<form>``` tag.

**Syntax of Form Element**

{% highlight html %}
<form>
...
Various input tags
...
</form>
{% endhighlight %}

## The ```<input>``` Tag
The ```<input>``` element is most important element to make forms in html.

The input element can have various forms that depens on text attribute:-

Some common types of input elements.
1. **text** :- Used to define text field.
2. **radio** :- Used to select one of many choices.
3. **checkbox** :- Used to select Multiple choice.
4. **submit** :- Used to define submitt button for the forms data.
5. **password** :- Used to define password field.
6. **date**:- used to define date field

### Example of Simple form

{% highlight html %}
<form action="">
  First name:<br>
  <input type="text" name="firstname"><br>
  Last name:<br>
  <input type="text" name="lastname"><br>
  email:<br>
  <input type="email" name="email"><br>
  password:<br>
  <input type="password" name="password"><br>
  <input type="submit" value="Submit">
</form>
{% endhighlight %}

[DEMO](https://codepen.io/riwajchalise/pen/xxxpNBw)

## The <fieldset> and <legend> tags.
The ```<fieldset>``` is used to group related date in a form and the ```<legend>``` tag is used to define the csption fo the fieldset. 

### Examples of forms using ```<fieldset>``` and ```<legend>```
{% highlight html %}
<form action="">
  <fieldset>
    <legend>Fill the Form:</legend>
<form action="/action_page.php">
  First name:<br>
  <input type="text" name="firstname"><br>
  Last name:<br>
  <input type="text" name="lastname"><br>
  email:<br>
  <input type="email" name="email"><br>
  password:<br>
  <input type="password" name="password"><br>
  <input type="submit" value="Submit">
</form>
  </fieldset>
</form>
{% endhighlight %}

[DEMO](https://codepen.io/riwajchalise/pen/vYYpwoZ)

You can use various CSS properties to design a form.




