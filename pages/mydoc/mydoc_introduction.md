---
title: Introduction and prerequisites
sidebar: mydoc_sidebar
permalink: mydoc_introduction.html
folder: mydoc
summary: This is brief instruction about the requirments that you need to have before starting the course
---

## Installations
You need to have following requirments to run php on your local machine


### 1. Setup PHP 

#### For Windows

XAMPP stands for Cross-Platform (X), Apache (A), MariaDB (M), PHP (P) and Perl (P). It is a simple, lightweight Apache distribution that makes it extremely easy for developers to create a local web server for testing and deployment purposes

You can download xampp [here](https://www.apachefriends.org/index.html) 

#### For Linux (Ubuntu)

Install Apache using the following commands

```
sudo apt-get update
sudo apt-get install apache2
```

Install PHP

```
sudo apt-get install php
```

Remove the default page of apache

```
sudo mv /var/www/html/index.html /var/www/html/index.back
```

Open a new file named 

```
sudo nano /var/www/html/index.php
```

Paste the following code in the file and press ctrl + x and then Y to save and exit the file
{% highlight php %}
<?php
print_r (phpinfo());
?>
{% endhighlight %}


Finally restart the apache2 server
```
sudo systemctl restart apache2
```

### 2. Download and Install a code editor

You can have one of these editors to write/edit your code:-

* [Visual code studio](https://code.visualstudio.com/) 

* [Atom](https://atom.io)

* [Sublime-Text](https://www.sublimetext.com/)

You can also use other tools as per your prefrence.

## Version Control

### 1. Github account
[GitHub](https://github.com/) is a web-based hosting service for software development projects that use the Git revision control system.

For beginners it can be a best place to store your code. Learning about version control system in the earlier phase of programming can give you a head-start later phase of coding and developement.

### 2. Git Cli (Gitbash for windows)
[Git-Bash](https://git-scm.com/downloads) is an application for Microsoft Windows environments which provides an emulation layer for a Git command line experience. Bash is a popular default shell on Linux and macOS.

{% include note.html content="You don't have to download git bash if you use Mac or Linux as your main operating system." %}


{% include links.html %}
