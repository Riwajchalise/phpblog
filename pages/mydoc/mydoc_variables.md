---
title: Variables
keywords: variables,php variables
last_updated: November 7, 2019
summary: "This post will help you understand what are variables and how to make variables in php."
sidebar: mydoc_sidebar
permalink: mydoc_variables.html
folder: mydoc
datatable: true
---

Variable is a name that has a value associated with it. Variables are used to store values such as strings, numeric values, characters or memory address.

## Declaring variables in PHP
Variables in PHP start with a ```$``` sign followed by the name of the variable.

For a variable to be valid the variable name must start with alphabet (a-z or A-Z) or underscore (_), followed by numbers, letters or underscore.

There cannot be white space in variable so if the variable has more than oneo word it is seperated by commas (for example ```$two_words``` , ```deer_walk```)

## Some Valid PHP Variables

Here are some valid php variables:

### Example-1
{% highlight php %}

<?php
$xyz = 'welcome';
$XYZ = 'welcome';
$Xyz = 'welcome';
$xyz1231 = 'welcome';
$xyZ = 'welcome';
$XYZ = 'welcome';
$_XYZ = 'welcome';
$XYZ_xyz = 'welcome';
?>

{% endhighlight %}

[DEMO](https://paiza.io/projects/3jAW7zBhvprgs-1oR5q5gQ?language=php)

{% include important.html content="PHP variables are case sensitive." %}

### Example-2(Operation)

{% highlight php %}
<?php
$x = 20;
$y = 30;
echo $x + $y;
?>
{% endhighlight %}

[DEMO](https://paiza.io/projects/3jAW7zBhvprgs-1oR5q5gQ?language=php)

## PHP: A loosly typed language
PHP automatically detects the datatype of the variable by the type of value we give the variable.

The data type is not set in strict manner, that means you can do things like adding strings to intiger without causing an error.

However, PHP 7 allows user to assigne datatype by enabling strict. This gives an option to declare datatype while assigning a variable.

{% highlight php %}

<?php
$a = 2;
$b = 2.33;

echo $a + $b;
?>

{% endhighlight %}

[DEMO](https://paiza.io/projects/Aydehq0VGnCqfY-s5DYwrQ?language=php)


