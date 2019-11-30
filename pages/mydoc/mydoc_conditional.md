---
title: Conditional Statement
keywords: if, else, if_else, if_elseif
last_updated: November 30, 2019
tags: 
summary: "This post will help you understand conditional logic in PHP"
sidebar: mydoc_sidebar
permalink: mydoc_conditional.html
folder: mydoc
---
Conditional statements are used to perform actions based on conditions.

Types of conditional statements in PHP:-
1. if statement
2. if...else statement
3. if...elseif...else statement
4. switch statement

## if Statement
The ```if``` statement executes codes if one condition is true.

### Syntax
```
if (condition) {
    //code;
}
```
### Example
{% highlight php %}
<?php
$t = 20;

if ($t == "20") {
    echo "I have Rs. 20";
}
?>
{% endhighlight %}
[DEMO](https://paiza.io/projects/aA8rD9Qpr6n2o2xg3rD-OA?language=php)

## if...else Statement
The ```if...else``` statement executes some code if the condition is true and another code if the condition is false.

### Syntax
```
if (condition) {
   // code1
} else {
   // code2;
}
```

### Example
{% highlight php %}
<?php
$t = 10;

if ($t == "20") {
    echo "I have Rs. 20";
} else {
    echo "I don't have Rs. 20";
}
?>
{% endhighlight %}
[DEMO](https://paiza.io/projects/EYyGG7P6a5sy5JXre2bwvA?language=php)


## if...elseif...else Statement
If there are more than one condition then we can use ```if...elseif...else``` condition.

### Syntax

```
if (condition) {
    //code1
} elseif (condition) {
    //code2
} else {
    //code3 
}
```

### Example

{% highlight php %}
<?php
$t = 10;

if ($t == "20") {
    echo "I have Rs. 20";
} elseif($t < 20) {
    echo "I have less than Rs. 20";
} else{
    echo "I have more than Rs. 20";
}
?>
{% endhighlight %}

[DEMO](https://paiza.io/projects/5iyG145eUr_PJHaQQRaiAw?language=php)