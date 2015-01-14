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

### 4.3 get(path: String, getSuccess: () -> Void)
Uses Backend.BASE_URL + path to obtain a full url to get the cases array. This url is used in the request which the function does. It get's an array with json items and will send to `self.delegate.didReceiveAPIResults(jsonResult)`.

##### Example of the json result:
```swift
[
    {
        id: 9,
        title: "Verbetering van het imago rondom Groningen",
        status: "In progress",
        casetype: "RFA",
    },
    {
        id: 8,
        title: "Instemmingsverzoek tot online video marketing",
        status: "Open",
        casetype: "RFC",
    },
    {
        id: 1,
        title: "Aardbevingen rondom Ten Boer",
        status: "Open",
        casetype: "NFI",
    },
    {
        id: 5,
        title: "Contactpersonen Shell",
        status: "Closed",
        casetype: "Info",
    }
]
```

### 4.4 getAllCases(success: () -> Void) -> Void
Is the callback function of the get function.


