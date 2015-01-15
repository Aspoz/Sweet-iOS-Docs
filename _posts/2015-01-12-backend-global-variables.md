---
layout: page
title: "2. Global Variables"
category: back
date: 2015-01-12 16:28:00
---

In the `class Backend` are global variables defined that are accessable to inhertited classes. You will find a list of all global variables in this document.

### BASE_URL
Returns a `String` that contains the API URL.

##### Example:
```swift
  var string_url = BASE_URL + "/cases"
  print_ln(string_url)
```

##### Returns:
```swift
  "http://178.62.204.157/cases"
```
