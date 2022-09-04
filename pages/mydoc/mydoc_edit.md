<!-- ---
title: Update(Edit) Data from Database
keywords: datatypes, datatype
last_updated: March 29, 2020
summary: "This post will help you understand how to edit data from database."
sidebar: mydoc_sidebar
permalink: mydoc_update.html
folder: mydoc
datatable: true
---

## Edit 
In refrence to previous post (retrive) we will now understand how to edit data from database.

### edit.php

{% highlight php %}
<?php
// including the database connection file
include_once("config.php");

if(isset($_POST['update']))
{	

	$id = mysqli_real_escape_string($mysqli, $_POST['id']);
	
	$name = mysqli_real_escape_string($mysqli, $_POST['name']);
	$age = mysqli_real_escape_string($mysqli, $_POST['age']);
	$message = mysqli_real_escape_string($mysqli, $_POST['message']);	
	
	
		//updating the table
		$result = mysqli_query($mysqli, "UPDATE users SET name='$name',age='$age',message='$message' WHERE id=$id");
		
		//redirectig to the display page. In our case, it is index.php
		header("Location: index.php");
	
}
?>

<?php
//getting id from url
$id = $_GET['id'];

//selecting data associated with this particular id
$result = mysqli_query($mysqli, "SELECT * FROM users WHERE id=$id");

while($res = mysqli_fetch_array($result))
{
	$name = $res['name'];
	$age = $res['age'];
	$message = $res['message'];
}
?>
<html>
<head>	
	<title>Edit Data</title>
</head>

<body>
	<a href="index.php">Home</a>
	<br/><br/>
	
	<form name="form1" method="post" action="edit.php">
		<table border="0">
			<tr> 
				<td>Name</td>
				<td><input type="text" name="name" value="<?php echo $name;?>"></td>
			</tr>
			<tr> 
				<td>Age</td>
				<td><input type="text" name="age" value="<?php echo $age;?>"></td>
			</tr>
			<tr> 
				<td>Email</td>
				<td><input type="text" name="message" value="<?php echo $message;?>"></td>
			</tr>
			<tr>
				<td><input type="hidden" name="id" value=<?php echo $_GET['id'];?>></td>
				<td><input type="submit" name="update" value="Update"></td>
			</tr>
		</table>
	</form>
</body>
</html>

{%endhighlight%}

- First the database file is included once. 
- Then we retrive the data from database and display in the form. 
- Then the form value can be edited and updated. -->
