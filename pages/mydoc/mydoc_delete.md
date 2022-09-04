<!-- ---
title: Data Types
keywords: datatypes, datatype
last_updated: March 29, 2020
summary: "This post will help you understand how to delete data from database."
sidebar: mydoc_sidebar
permalink: mydoc_delete.html
folder: mydoc
datatable: true
---

## Delete
In the previous data we selected data from the database. In refrence to previous post we will now understand how to delete data from database.

### delete.php

{% highlight php %}
<?php
//including the database connection file
include("config.php");

//getting id of the data from url
$id = $_GET['id'];

//deleting the row from table
$result = mysqli_query($mysqli, "DELETE FROM users WHERE id=$id");

//redirecting to the display page (index.php in our case)
header("Location:index.php");
?>
{% endhighlight %}

In above code:-
- We first include the database file.
- Get the id of row to be deleted.
- Apply the delete query to delete the data.
- redirect to index.php -->