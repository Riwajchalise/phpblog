<!-- ---
title: Database Connection
keywords: Database, Database_Connection_In_PHP
last_updated: March 3, 2020
tags:
summary: "This post describes how mysqli database is connected in PHP."
sidebar: mydoc_sidebar
permalink: mydoc_db_connection.html
folder: mydoc
---

## MYSQLi

The MySQLi Extension ( MySQL Improved) is a relational database driver used in the PHP programming language to provide an interface with MySQL databases. In this tutorial we will use MySQLi driver since it provides procedual and OOP interface.

## Databasse Connection

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

{% include callout.html content="
when you install XAMPP in your windows machine, the root password for the MySQL is set to empty. But this is not recommended, as the MySQL database without a password will be accessible to everyone. To avoid this, a proper/secure password must be set to the user root 
" type="primary" %} -->
