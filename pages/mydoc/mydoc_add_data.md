---
title: Adding Data Using Form.
keywords: adding data
last_updated: March 30, 2020
tags:
summary: "Adding data on database using form"
sidebar: mydoc_sidebar
permalink: mydoc_add_data.html
folder: mydoc
---

## Database Connection

Database connection is very important while playing with any of the CRUD operation. Name the Database file `config.php`.

Download and import the database.

<a target="\_blank" class="noCrossRef" href="test.sql"><button type="button" class="btn btn-default" aria-label="Left Align"><span class="glyphicon glyphicon-download-alt" aria-hidden="true"></span>Download Database</button></a>

### config.php

{% highlight php %}

<?php


$databaseHost = 'localhost';
$databaseName = 'test';
$databaseUsername = 'root';
$databasePassword = '';

$mysqli = mysqli_connect($databaseHost, $databaseUsername, $databasePassword, $databaseName); 
 
?>

{% endhighlight %}

## HTML Form

Add the following HTML form. The form has Http method post and the action as add.php. This form contain three different inputs:-

- Name
- Age
- Message

### add.html

{% highlight php %}

<html>
  <head>
    <title>Add Data</title>

  </head>

  <body>
    <a href="index.php">Home</a>
    <br /><br />

    <form action="add.php" method="post" name="form1">
      <table width="25%" border="0">
        <tr>
          <td>Name</td>
          <td><input type="text" name="name" /></td>
        </tr>
        <tr>
          <td>Age</td>
          <td><input type="text" name="age" /></td>
        </tr>
        <tr>
          <td>Message</td>
          <td>
            <textarea type="text" name="message" rows="10" cols="50"></textarea>
          </td>
        </tr>
        <tr>
          <td></td>
          <td><input type="submit" name="Submit" value="Add" /></td>
        </tr>
      </table>
    </form>

  </body>
</html>
{% endhighlight %}

## PHP Code

This file handles the data entered by the users.

### add.php

{% highlight php %}

<?php
//including the database connection file
include_once("config.php");

if (isset($_POST['Submit'])) {
	$name = mysqli_real_escape_string($mysqli, $_POST['name']);
	$age = mysqli_real_escape_string($mysqli, $_POST['age']);
	$message = mysqli_real_escape_string($mysqli, $_POST['message']);



	$result = mysqli_query($mysqli, "INSERT INTO users(name,age,message) VALUES('$name','$age','$message')");

	//display success message
	echo "<font color='green'>Data added successfully.";
	echo "<br/><a href='index.php'>View Result</a>";
}
?>
{% endhighlight %}

In the above code:

- First the data from the foms are captured.
- If the fields are not empty the data are inserted in database.
- Then display screen is shown.
