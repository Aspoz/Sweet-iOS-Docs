---
layout: page
title: "5. String"
category: ext
date: 2015-01-12 16:28:00
---

### 5.1 formatDate()

This method can be ran on a `String` with a date in the following format: `"yyyy-MM-dd'T'HH:mm:ss.SSS'Z'"` and will be formatted into: `HH:mm' - 'dd MMM yyyy`. This function will also return a `String`.

##### Dependence:
Requires the private `turnDateIntoString()` function

##### Example:
```swift
  let dateFromAPI = "2014-12-11T08:47:18.594Z"

  dateFromAPI.formatDate()
```

##### Result:
```swift
  "08:47 - 11-12-2014"
```
