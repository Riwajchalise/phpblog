<!-- ---
title: For Loop
keywords: for_loop, for, php
last_updated: December 10, 2019
tags: 
summary: "This post describes the conceptof for loop in php"
sidebar: mydoc_sidebar
permalink: mydoc_for_loop.html
folder: mydoc
---

## What is a Loop?
In computer science, a loop is a programming structure that repeats a sequence of instructions until a specific condition is met.

## For loop
For loop is used to run a specific set of code until the specified number of times.

### Syntax 

```
for (initialization; condition; increment){
   code to be executed;
}
```

### Example1

A simple for loop program to print number from 0 to 10
 
{% highlight php %}
<?php 
for ($x = 0; $x <= 10; $x++) {
    echo "The number is: $x <br>";
} 
?>
{% endhighlight %}
[DEMO](https://paiza.io/projects/a2G9uOGAljOFNh3__5W8zA)

Here in this example:
* $x = 0 initilization
* $x <= 10 Condition
* $x++ Increases the loop value counter by 1

### Example2

A simple program to print the table of 2;

{% highlight php %}
<?php 
for ($x = 1; $x <= 10; $x++) {
    $b = 2 * $x;
    echo "2 * " .  $x . "= ". $b. "\n";
} 
?>
```
{% endhighlight %}

[DEMO](https://paiza.io/projects/vLcbaWhMJjvp5-Ihi8Lc7g?language=php) -->