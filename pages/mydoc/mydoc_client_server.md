---
title: Software Architecture
keywords: Database, datbase_intro
last_updated: September 4, 2022
tags: 
sidebar: mydoc_sidebar
permalink: mydoc_client_server.html
folder: mydoc
---

Software Architecture consists of One Tier, Two Tier, Three Tier, and N-Tier architectures.

A “tier” can also be referred to as a “layer”.

Three layers are involved in the application namely Presentation Layer, Business Layer, and Data Layer. Let’s see each layer in detail:

## 1. Presentation Layer
It is also known as the Client layer. The top most layer of an application. This is the layer we see when we use the software. By using this layer we can access the web pages. 

The functionality of Presentation layer is 
- To communicate with the Application layer. 
- This layer passes the information which is given by the user in terms of keyboard actions, mouse clicks to the Application Layer.

For example, the login page of Gmail where an end-user could see text boxes and buttons to enter user id, password, and to click on sign-in.

## 2. Application Layer

It is also known as Business Logic Layer which is also known as the logical layer. As per the Gmail login page example, once the user clicks on the login button, the Application layer interacts with the Database layer and sends required information to the Presentation layer. It controls an application’s functionality by performing detailed processing. This layer acts as a mediator between the Presentation and the Database layer. Complete business logic will be written in this layer.

The functionality of Presentation layer is 
- TO Handle logical operation of the application.
- Communicate with the database to get request and send response to the client.

In simple words, it is to perform operations on the application.

## 3. Data Layer
The data is stored in this layer. The application layer communicates with the Database layer to retrieve the data.

The functionality of Presentation layer is:
- To Perform database operation (insert, update, delete)


# Types of Software Architecture

## One Tier Architecture:

One Tier application AKA Standalone application. One-tier architecture has all the layers such as Presentation, Business, Data Access layers in a single software package. Applications that handle all the three tiers such as MP3 player, MS Office come under the one-tier application. The data is stored in the local system or a shared drive. 

{% include image.html file="one-tier-software-architecture.png" alt="Jekyll" caption="One Tire Architecture" %}

## Two Tier Architecture:
Two Tier application AKA Client-Server application

The Two-tier architecture is divided into two parts:

1. Client Application (Client Tier)
2. Database (Data Tier)

The client system handles both Presentation and Application layers and the Server system handles the Database layer. It is also known as a client-server application. The communication takes place between the Client and the Server. The client system sends the request to the server system and the Server system processes the request and sends back the data to the Client System

{% include image.html file="two-tier-software-architecture.png" alt="Jekyll" caption="Two Tire Architecture" %}

## Three Tier Architecture:

Three Tier application AKA Web Based application

The Three-tier architecture is divided into three parts:

1. Presentation layer (Client Tier)
2. Application layer (Business Tier)
2. Database layer (Data Tier)

The client system handles the Presentation layer, the Application server handles the Application layer, and the Server system handles the Database layer.

{% include image.html file="three-tier-software-architecture.png" alt="Jekyll" caption="Three Tire Architecture" %}






