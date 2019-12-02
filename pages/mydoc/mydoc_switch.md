---
title: Switch
keywords: Switch, switch_case
last_updated: 
tags: 
summary: "This post will describe about Switch case in php."
sidebar: mydoc_sidebar
permalink: mydoc_switch.html
folder: mydoc
---

The ```switch``` statement in PHP can be used to perform differnet action based on different cases. If can be used as a substitute for if...elseif

## Syntax

```
switch (a) {
    case value1:
        code to be executed if a = value1;
        break;
    case var2:
        code to be executed if a=var2;
        break;
    ...
    default:
        code to be executed if a is different from all var;
}

```