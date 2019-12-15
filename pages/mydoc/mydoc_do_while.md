---
title: Do While loop
keywords: do_while
last_updated: 
tags: 
summary: "Tis post describes do while loop in PHP"
sidebar: mydoc_sidebar
permalink: mydoc_do_while.html
folder: mydoc
---

## D0...While
The ```do...while``` loop will always execute the block of code once, then check the condition, and repeat the loop until the specified condition is true.

```
do {
    #code;
} while (condition);
```
### Example
A program to print number from 1 to 10 using do_while.

{% highlight php %}
<?php 
$x = 1; 

do {
    echo "$x";
    $x++;
} while ($x <= 10);
?>
{% endhighlight %}
[DEMO](https://paiza.io/projects/C-4LsnmPaq2jqp7iGrZ1dA?language=php)




