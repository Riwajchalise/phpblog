<!-- ---
title: Adding Data Using Form.
keywords:
last_updated: March 5, 2020
tags:
summary: "Adding data on database using form"
sidebar: mydoc_sidebar
permalink: mydoc_add.html
folder: mydoc
---

## Database connection

Database connection is very important while playing with any of the CRUD operation. Name the Database file `config.php`.

### config.php

{% highlight php%}

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

## PHP code

This file handles the data entered by the users.

### add.php

{% highlight php %}
<html>
<head>
	<title>Add Data</title>
</head>

<body>
<?php
//including the database connection file
include_once("config.php");

if(isset($_POST['Submit'])) {	
	$name = mysqli_real_escape_string($mysqli, $_POST['name']);
	$age = mysqli_real_escape_string($mysqli, $_POST['age']);
	$message = mysqli_real_escape_string($mysqli, $_POST['message']);
		
	// checking empty fields
	if(empty($name) || empty($age) || empty($message)) {
				
		if(empty($name)) {
			echo "<font color='red'>Name field is empty.</font><br/>";
		}
		
		if(empty($age)) {
			echo "<font color='red'>Age field is empty.</font><br/>";
		}
		
		if(empty($message)) {
			echo "<font color='red'>Email field is empty.</font><br/>";
		}
		
		//link to the previous page
		echo "<br/><a href='javascript:self.history.back();'>Go Back</a>";
	} else { 
		// if all the fields are filled (not empty) 
			
		//insert data to database	
		$result = mysqli_query($mysqli, "INSERT INTO users(name,age,message) VALUES('$name','$age','$message')");
		
		//display success message
		echo "<font color='green'>Data added successfully.";
		echo "<br/><a href='index.php'>View Result</a>";
	}
}
?>
</body>
</html>

{% endhighlight %}

In the above code:
- first the data from the foms are captured.
- Then the code checks for empty fields.
- If the fields are not empty the data are inserted in database.
- Then display Screen is shown. -->