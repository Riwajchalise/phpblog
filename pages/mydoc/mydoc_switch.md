---
title: Switch
keywords: Switch, switch_case
last_updated: 
tags: 
summary: "This post will describe about Switch case in php."
sidebar: mydoc_sidebar
permalink: mydoc_switch.html
folder: mydoc
---

The ```switch``` statement in PHP can be used to perform differnet action based on different cases. If can be used as a substitute for if...elseif

## Syntax

```
switch (a) {
    case value1:
        code to be executed if a = value1;
        break;
    case var2:
        code to be executed if a=var2;
        break;
    ...
    default:
        code to be executed if a is different from all var;
}

```

### Understading The Syntax

* There are a number of expressions (variables).
* There are number of cases.
* The case and expression is checked, if there is a match the block of code associated with the case is executed.
* The ```break``` statement prevent the code from running into the next case automatically.
* The code segment ```default``` case is executed if no match is found.


## Example

{% highlight php %}
<?php
$num = 3;
 
switch ($num) {
    case 1:
        echo "Your favorite number is 1";
        break;
    case 2:
        echo "Your favorite number is 2";
        break;
    case 3:
        echo "Your favorite number is 3";
        break;
    default:
        echo "Your favorite number is not mentioned";
}
?>
{% endhighlight %}

[DEMO](https://paiza.io/projects/RO78jWHYU6hW-nwZTsbegg?language=php)