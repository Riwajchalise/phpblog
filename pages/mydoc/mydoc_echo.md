<!-- ---
title: echo
keywords: echo, php print
last_updated: October 31, 2019
summary: "This post will help you understand how to use echo() function on php."
sidebar: mydoc_sidebar
permalink: mydoc_echo.html
folder: mydoc
datatable: true
---

echo is a php function that can be used to print one or many string.

## Syntax of echo

{% highlight php %}
echo (string);
{% endhighlight %}

### Example-1 
A simple echo statement

{% highlight php %}
<?php
echo "Welcome to php class.";
?>
{% endhighlight %}

[DEMO](https://paiza.io/projects/WDNxhzHFIVGUYK4OrWwf9A)

You can also print variables

### Example-2 (Variables)
You can also print variables. 

{% include important.html content="PHP variables will be discussed later in the documentation. For now just know that a php variable starts with a ```$``` sign." %}

{% highlight php %}
<?php
$str = "Welcome to PHP Class";
echo $str;
?>
{% endhighlight %}

[DEMO](https://paiza.io/projects/RLCZynaYO7yV8dAqPIvVJw?language=php)

### Example-3 (HTML tags)
You can also embed HTML tags in the echo  statement.

{% highlight php %}
<?php
echo "<h1>This is h1 tag</h1>";
echo "<p>This is p tag</p>";
?>
{% endhighlight %}

[DEMO](https://paiza.io/projects/rqEG9Y3Yc1uAhqKythCIYQ?language=php)

### Example-4 (Joining)
You can join the two variables together by using ```.``` as a joining operator:-

{% highlight php %}
<?php
$str1 = "Welcome to";
$str2 = "PHP class";
echo $str1 . " " . $str2;
?>
{% endhighlight %}

[DEMO](https://paiza.io/projects/o6956HIHri0AkhL9NGEpEA?language=php)

{% include links.html %} -->
