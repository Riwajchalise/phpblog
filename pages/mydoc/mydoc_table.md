---
title: HTML tables 
keywords: HTML tables, tables in html, table design, HTML
last_updated: October 31, 2019
tags: 
summary: "This post will give you the brief introduction about HTML tables. However, It won't cover everything about HTML tables but just enough to use it for you PHP lesson."
sidebar: mydoc_sidebar
permalink: mydoc_table.html
folder: mydoc
datatable: true
---

A HTML table is defined by ```<table>``` tag.
The head is defined by ```<th>``` tag.
The row is defined by ```<tr>``` tag.
The data is defined with ```<td>``` tag.

Here is what a simple HTML table looks like:-

#### Example of simple table

{% highlight html %}
<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Charls</td>
    <td>Doe</td>
    <td>22</td>
  </tr>
  <tr>
    <td>Dudly</td>
    <td>Jons</td>
    <td>44</td>
  </tr>
</table>
{% endhighlight %}

[DEMO](https://codepen.io/riwajchalise/pen/oNNpjay)

However, we can add css properties to enhance the design of the table
{% highlight html %}
<head>
<style>
table, th, td {
  border: 1px solid black;
}
</style>
</head>
<body>
<table style="width:100%">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Charls</td>
    <td>Doe</td>
    <td>22</td>
  </tr>
  <tr>
    <td>Dudly</td>
    <td>Jons</td>
    <td>44</td>
  </tr>
</table>
{% endhighlight %}

[DEMO](https://codepen.io/riwajchalise/pen/qBBpbaJ)