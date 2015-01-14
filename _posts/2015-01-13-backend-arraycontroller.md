---
layout: page
title: "4. ArrayController"
category: back
date: 2015-01-12 11:43:03
---

The `class ArrayController` can use the following functions:

### 4.1 ArrayControllerProtocol
Protocol which makes sure `func didReceiveAPIResults`'s result is a NSArray.

##### Example:
You can find an init of the ArrayControllerProtocol in the overviewViewController.

### 4.2 Variables
```swift
var delegate: ArrayControllerProtocol
```
Defines type of variable 'delegate', which is a Protocol.

```swift
var backend = Backend()
```
Defines 'backend' as variable for the class [Backend](../back/backend-introduction.html).
