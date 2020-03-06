---
title: HTTP Method (GET and POST)
keywords: GET, POST
last_updated: March 3, 2020
tags:
summary: "This post describes the HTTP method (GET and POST) method."
sidebar: mydoc_sidebar
permalink: mydoc_get_and_post.html
folder: mydoc
---

## HTTP Method
HTTP defines methods to indicate the desired action to be performed on the identified resource. We have two methods for the shakke of understanding this tutorial.
- GET
- POST

### GET Method
Get method is used to request data from specific resource. In get method string value pairs are sent in the URL of a get request.

```
/test/demo_form.php?name=Raj&id=2
```

### POST method

POST is used to send data to a server to create/update a resource. The data sent to the server with POST is stored in the request body of the HTTP request:

```
POST /test/demo_form.php HTTP/1.1
Host: charlsphp.com
name=Raj&id=2
```




