---
title: Retrive Data From the Database
keywords: retrive, CRUD
last_updated: Mar 7, 2019
tags:
summary: "This post discusses about the retrival of data from the database."
sidebar: mydoc_sidebar
permalink: mydoc_select.html
folder: mydoc
---

## Retrival(Select)

The Following code shows the data in table format. It will fetch all the data from the database.

### index.php
{% highlight php %}

<?php
//including the database connection file
include_once("config.php");

//fetching data in descending order (lastest entry first)
$result = mysqli_query($mysqli, "SELECT * FROM users ORDER BY id DESC"); // using mysqli_query
?>

<html>
<head>	
	<title>Homepage</title>
</head>

<body>
<a href="add.html">Add New Data</a><br/><br/>

    <table width='80%' border=1px>

    <tr bgcolor='#CCCCCC'>
    	<td>Name</td>
    	<td>Age</td>
    	<td>Message</td>
    	<td>Delete</td>
    </tr>
    <?php
    while($res = mysqli_fetch_array($result)) {
    	echo "<tr>";
    	echo "<td>".$res['name']."</td>";
    	echo "<td>".$res['age']."</td>";
    	echo "<td>".$res['message']."</td>";
    	echo "<td><a href=\"delete.php?id=$res[id]\" onClick=\"return confirm('Are you sure you want to delete?')\">Delete</a></td>";
    }
    ?>
    </table>

</body>
</html>

{% endhighlight %}

In above code:-
- Data are fetched in decending order.
- While loop is used to display the record until the last record.
- The record is displayed in table format.