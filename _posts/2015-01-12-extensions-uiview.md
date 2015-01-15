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
  let view = UIView(frame: CGRect(x: 0, y: 0, width: 50, height: 50))
  let caseitem = CaseItem(id: 1, title: "Test case", casetype: "RFC", status: "Open")

  view.addStatusColor(caseitem)
```

##### Result:
![addStatusColorBlue Color](http://i.imgur.com/lgpz8cm.png "addStatusColor Result")



### 3.2 roundedCorners( radius: CGFloat )
This method can be ran on an `UIView` to change the radius of the corners.

##### Example:
```swift
  let view = UIView(frame: CGRect(x: 0, y: 0, width: 50, height: 50))
  view.backgroundColor = UIColor.blackColor()

  view.roundedCorners(5)
```

##### Result:
![roundedCorners](http://i.imgur.com/tDx7XT7.png "roundedCorners Result")



### 3.3 makeCircle()
This method can be ran on an `UIView` to make the corners round based on the `width` and `height` of the `UIView`.

##### Example:
```swift
  let view = UIView(frame: CGRect(x: 0, y: 0, width: 50, height: 50))
  view.backgroundColor = UIColor.blackColor()

  view.makeRound()
```

##### Result:
![makeRound()](http://i.imgur.com/q8sx755.png "makeRound() Result")
