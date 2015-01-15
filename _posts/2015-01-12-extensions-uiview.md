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



### 3.4 showElement()
This method sets alpha to `1` for the `UIView` where the method is called on.

##### Example:
```swift
  let view = UIView(frame: CGRect(x: 0, y: 0, width: 50, height: 50))
  view.backgroundColor = UIColor.blackColor()

  view.showElement()
```

##### Result:
![showElement()](http://i.imgur.com/suG4Qii.png "showElement() Result")



### 3.4 hideElement()
This method sets alpha to `0` for the `UIView` where the method is called on.

##### Example:
```swift
  let view = UIView(frame: CGRect(x: 0, y: 0, width: 50, height: 50))
  view.backgroundColor = UIColor.blackColor()

  view.hideElement()
```

##### Result:
A hidden UIView



### 3.4 applyPlainShadow()
This method adds a pre-defined shadow for the `UIView` where the method is called on.

It's important that the `UIView` where the shadow is being called on, must be a subview of another `UIView`. This parentview must be atleast bigger than the radius and the offset. Make sure to make the width of the superview atleast `8` wider (radius of 4 on both left and right sides of 4, so 4 + 4 = 8) and for the height make is atleast `6` higher (radius of 4 plus shadow offset of 2, so 4 + 2 = 6).

The pre-defined shadow has the following attributes:

- shadowColor: **Black**
- shadowOffset: **x: 0, y: 2**
- shadowOpacity: **0.2**
- shadowRadius: **4**


##### Example:
```swift

let superview = UIView(frame: CGRect(x: 0, y: 0, width: 58, height: 56))
let subview = UIView(frame: CGRect(x: 4, y: 0, width: 50, height: 50))
subview.backgroundColor = UIColor.blackColor()

subview.applyPlainShadow()

superview.addSubview(subview)
```

##### Result:
![applyPlainShadow()](http://i.imgur.com/hKCiZPy.png "applyPlainShadow() Result")



### 3.4 applyCustomShadow( shadowWidth: Int, shadowHeight: Int, radius: CGFloat )
This method gives the developer the freedom to apply a customizable shadow to the `UIView` where the method is called on, but still keeps structure from the designer. The attributes `shadowOpacity` and `shadowColor` are not customizable.

It's important that the `UIView` where the shadow is being called on, must be a subview of another `UIView`. This parentview must be atleast bigger than the radius and the offset. Make sure to make the width of the superview is atleast bigger than the radius plus the offset. For more information, see the example down below.

The pre-defined shadow has the following attributes:

- shadowColor: **Black**
- shadowOffset: **x: shadowWidth, y: shadowHeight**
- shadowOpacity: **0.2**
- shadowRadius: **radius**


##### Example:
```swift

let superview = UIView(frame: CGRect(x: 0, y: 0, width: 58, height: 100))
let subview = UIView(frame: CGRect(x: 4, y: 6, width: 50, height: 50))
subview.backgroundColor = UIColor.blackColor()

subview.applyCustomShadow(0, shadowHeight: -2, radius: 4)

superview.addSubview(subview)
```

##### Result:
![applyCustomShadow()](http://i.imgur.com/7CvtevB.png "applyCustomShadow() Result")

