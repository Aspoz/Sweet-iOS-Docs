---
layout: page
title: "3. UIView"
category: ext
date: 2015-01-12 16:29:00
---

### 3.1 addStatusColor( caseItem: CaseItem )
This method can be ran on an `UIView` to add the corresponding case status color as `backgroundColor`.

##### Dependence:
Requires `Colors extension` and `class CaseItem`

##### Example:
```swift
  caseitem = CaseItem.new(1, title: "Test case", casetype: "RFC", status: "Open")

  UIView.addStatusColor(caseitem)
```

##### Result:
![addStatusColorBlue Color](http://i.imgur.com/lgpz8cm.png "addStatusColor Result")
