<!-- ---
title: Data Types
keywords: datatypes, datatype
last_updated: November 11, 2019
summary: "This post will help you understand datatypes in php."
sidebar: mydoc_sidebar
permalink: mydoc_datatypes.html
folder: mydoc
datatable: true
---

Variables store different datatypes like string, intiger, float, boolean, array.

{% include note.html content="var_dump() is a function that returns datatype and value." %} 

## String
A string is a group of characters put together, like "deer walk":

A string is always assigned inside a duble or a single quote:-

{% highlight php %}
<?php
$name = "Class of 2022";
var_dump($name)
?>
{% endhighlight %}

[DEMO](https://paiza.io/projects/MWiwU8AQXBix93fbkQQ08w?language=php)

## Integer
Integer is a datatype with non-decimal numbers. A integer can be either Positive or negetive. Arthmatic opreations can be performed on intigers. 

{% highlight php %}
<?php
$x = 5985;
$y = 2722;
$z = $x + $y;
var_dump($z);
?>
{% endhighlight %}
[DEMO](https://paiza.io/projects/qWSHhGQiwCeiHeN0-9wGRg?language=php)

## Float
A float is a number with decimal or exponential value.

{% highlight php %}
<?php 
$x = 12.124;
var_dump($x);
?>
{% endhighlight %}
[DEMO](https://paiza.io/projects/gLH7Eys3k8nxEccLOZbKeQ)


## Boolean
Boolean is used in conditional testing to test if the statement is True or False.

{% highlight php %}
<?php
$true = true;
$false = false;

var_dump($true);
var_dump($false);
?>
{% endhighlight %}

[Demo](https://paiza.io/projects/LswtpZoNv3qHnfKuY6qHdw)


## Array
Array is used to store multiple valued in a single variable.

{% highlight php %}
<?php 
$company = array("google","facebook","twitter");
var_dump($company);
var_dump($company[0]);
var_dump($company[1]);
var_dump($company[2]);
?>
{% endhighlight %}

[DEMO](https://paiza.io/projects/ck82yEhlbQ08KHU-IGa9xA?language=php)

There are more datatypes. For more information on datatypes check out [w3school](https://www.w3schools.com/php/php_datatypes.asp).

 -->
