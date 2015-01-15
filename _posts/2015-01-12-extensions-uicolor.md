---
layout: page
title: "2. UIColor"
category: ext
date: 2015-01-12 16:30:00
---

### 2.1 Colors
This extension contains all re-usable NAM colours and can be ran on `UIColor`.

##### Dependence:
Requires `colorWithRGBHex extension`

##### UIColor.namGreenColor()
Returns the `UIColor` object with the NAM Green colour.

##### UIColor.namBlueColor()
Returns the `UIColor` object with the NAM Blue colour.

##### UIColor.contentColor()
Returns the `UIColor` object with the main content colour.

##### UIColor.inProgressCaseColor()
Returns the `UIColor` object with the in progress case colour. Currently makes use of `namGreenColor()`

##### UIColor.openCaseColor()
Returns the `UIColor` object with the open case colour.

##### UIColor.closedCaseColor()
Returns the `UIColor` object with the closed case colour.

##### UIColor.caseSelectedColor()
Returns the `UIColor` object with the background color that is used for when a case is pressed or selected.

##### Example:
```swift
  let view =  UIView(frame: CGRect(x: 0, y: 0, width: 50, height: 50))

  view.backgroundColor = UIColor.namGreenColor()
```

##### Result:
![namGreenColor](http://i.imgur.com/C8AuRaD.png "namGreenColor Result")




### 2.2 colorWithRGBHex( hex: Int, alpha: Float = 1.0 )
This extension builds a `UIColor` object color from HEX. Fill in the `0x` plus HEX color code as a param for hex. If you want to change the opacity (alpha) of the color, add a param called `alpha` which can be filled with a `Float`

##### Example:
```swift
  // Make UIView background color #555555
  UIView.backgroundColor = UIColor.colorWithRGBHex(0x555555)

  // Make UIView background color #555555 with alpha 0.5
  UIView.backgroundColor = UIColor.colorWithRGBHex(0x555555, alpha: 0.5)
```

##### Result:
![contentColor](http://i.imgur.com/7AFZzmS.png "contentColor Result")

![contentColor](http://i.imgur.com/mIwoTuT.png "contentColor Result")
