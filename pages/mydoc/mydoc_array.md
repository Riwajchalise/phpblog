---
title: DUMMY
keywords: duummy.Dummy, Dummy text
last_updated: 
tags: 
summary: "This post will help to understand array in php."
sidebar: mydoc_sidebar
permalink: mydoc_array.html
folder: mydoc
---

## Array
Array is a variable that can store multiple values. In php `array()` function is used to make an array.

### Example

{% highlight php %}
<?php
$bikes = array("RC", "CRF", "DUKE");
echo "I like " . $bikes[0] . ", " . $bikes[1] . " and " . $bikes[2] . ".";
?>
{% endhighlight %}
[DEMO](https://paiza.io/projects/UbjT1VuL2lbO8IIYmM7tDg)

## Types of Array
The types of array are:-
- Indexed Arrays   
- Associative Arrays  
- Multidimentional Arrays  

### Indexed Arrays
An index in an array is a unique value that is used to identify a value of an array. The index always starts from 0.

**Index can be assigned automatically:-**
```
$bikes = array("RC", "CRF", "DUKE");
```

**Index can be assgned manually:-**
```
$cars[0] = "Volvo";
$cars[1] = "BMW";
$cars[2] = "Toyota";
```

#### Looping in Indexed array
Here we use for loop to loof through ndexed array.

{% highlight php %}

<?php
$bikes = array("RC", "CRF", "DUKE");
$arrlength = count($bikes);

for($x = 0; $x < $arrlength; $x++) {
    echo $bikes[$x];
    echo "<br>";
}
?>

{% endhighlight %}
[DEMO](https://paiza.io/projects/ilpaOxI0iYUUtzhwFnWHEg)


### Associative Arrays

Associative arrays are arrays that use named keys that you assign to them.

```
$bikes = array("KTM"=>"RC", "Honda"=>"CRF", "KTM2"=>"DUKE");
```

#### Looping in Associative Array
{% highlight php %}
<?php
$bikes = array("KTM"=>"RC", "Honda"=>"CRF", "KTM2"=>"DUKE");

foreach($bikes as $x => $x_value) {
    echo "Key=" . $x . ", Value=" . $x_value;
    echo "<br>";
}
?>
{%endhighlight%}

[DEMO](https://paiza.io/projects/eBHTaTKRT6cK7Ok6DF1G6g?language=php)

### Multidimensional Arrays

A multidimensional array is an array containing one or more arrays.

```
$bikes = array
  (
  array("RC",56,34),
  array("DUKE",12,6),
  array("CRF",4,2),
  array("Pulser",13,11)
  );
```

#### Presentation of Multidimensional Array
{%highlight php%}
<?php
$bikes = array
  (
  array("RC",56,34),
  array("DUKE",12,6),
  array("CRF",4,2),
  array("Pulser",13,11)
  );
  
echo $bikes[0][0].": In stock: ".$bikes[0][1].", sold: ".$bikes[0][2].".<br>";
echo $bikes[1][0].": In stock: ".$bikes[1][1].", sold: ".$bikes[1][2].".<br>";
echo $bikes[2][0].": In stock: ".$bikes[2][1].", sold: ".$bikes[2][2].".<br>";
echo $bikes[3][0].": In stock: ".$bikes[3][1].", sold: ".$bikes[3][2].".<br>";
?>
{% endhighlight %}

[DEMO](https://paiza.io/projects/rii0w9BTG-THt-fz8WUd7A?language=php)

