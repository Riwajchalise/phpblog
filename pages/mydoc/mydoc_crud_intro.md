<!-- ---
title: Introduction to CRUD Operation
keywords: CRUD, CRUD_OPERATION
last_updated: March 3, 2020
tags:
summary: "This post describes CRUD operation in PHP and MySql."
sidebar: mydoc_sidebar
permalink: mydoc_crud_intro.html
folder: mydoc
---

CRUD stands for create read update and delete of data in database.

## DB connection

It is very important to connect to database for each of crud operation. So first we make a database file named `config.php` and add the object everytime we perform one of the CRUD operations. `include_once()` method is used to add the database object.

{% highlight php %}

<?php
$servername = "localhost";
$username = "root"; 
$password = "";
$dbname = "test";

// Create database connection
$conn = new mysqli($servername, $username, $password, $dbname);

// Check connection
if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}
echo "Connected successfully";
?>

{% endhighlight %}

## Create

Execute the followig code to create a table named `message` in the database.

{% highlight php %}

<?php

include_once("db.php");

$sql = "Create table message 
	(Name varchar(30), 
	Email varchar(30), 
	Message varchar(500)
	)";

if ($conn->query($sql) === TRUE) {
    echo "New table created";
} else {
    echo "Error: " . $sql . "<br>" . $conn->error;
}

$conn->close();
?>

{% endhighlight %}

## Insert

Executing the code below will insert a record in the table created.

{% highlight php %}

<?php

include_once("config.php");

$sql = "INSERT INTO message (Name, Email, Message)
VALUES ('John', 'john@example.com', 'this is a message')";

if ($conn->query($sql) === TRUE) {
    echo "New record created successfully";
} else {
    echo "Error: " . $sql . "<br>" . $conn->error;
}

$conn->close();
?>

{% endhighlight %}

## Read

Executing the code below will show/retrive the record.

{% highlight php %}

 <?php

include_once("db.php");

$sql = "SELECT Name, Email, Message from message";
$result = $conn->query($sql);

if ($result->num_rows > 0) {
    // output data of each row
    while($row = $result->fetch_assoc()) {
        echo "<br> Name: ". $row["Name"]. " - Email: ". $row["Email"]. " " .  " -Message:" . $row["Message"] . "<br>";
    }
} else {
    echo "no results";
}

$conn->close();
?>

{% endhighlight %}

## Update

Executing the code below will update the email of the records name John.

{% highlight php%}

<?php

include_once("db.php");

$sql = "UPDATE message SET Email = 'wa@php.m' where Name = 'John' ";

if ($conn->query($sql) === TRUE) {
    echo "Updated successfully";
} else {
    echo "Error: " . $sql . "<br>" . $conn->error;
}

$conn->close();
?>

{% endhighlight %}

## Delete

Executing thec code below will delete the record.

{% highlight php %}

<?php

include_once("db.php");

$sql = "DELETE FROM message WHERE Name = 'John'";

if ($conn->query($sql) === TRUE) {
    echo "Deleated Successfully";
} else {
    echo "Error: " . $sql . "<br>" . $conn->error;
}

$conn->close();
?>

{% endhighlight %}

In the next article we will perform these operation by creating a user interface. -->
