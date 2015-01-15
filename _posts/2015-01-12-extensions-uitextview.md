---
layout: page
title: "4. UITextView"
category: ext
date: 2015-01-12 16:28:00
---

### 4.1 addPlaceholderIfEmpty( message: String )
This method can be ran on an `UITextView` to add placeholder text as `message` and remove it on the next call of the same function on the same instance. This can be perfectly used for `textViewDidBeginEditing` and `textViewDidEndEditing` events, to add and remove placeholder text.

##### Example:
```swift
  let textview = UITextView(frame: CGRect(x: 0, y: 0, width: 200, height: 100))
  textview.backgroundColor = UIColor.cyanColor()

  textview.addPlaceholderIfEmpty("Add your text here...")
```

##### Result:
![addPlacholderIfEmpty Color](http://i.imgur.com/ZH9mJYh.png "addPlaceholderIfEmpty Result")

If this function is ran again on the same instance of the `UITextView`, the placeholder will be removed.

![addPlacholderIfEmpty Color](http://i.imgur.com/YKEJb1A.png "addPlaceholderIfEmpty Result")
