---
layout: page
title: "4. Models"
category: front
date: 2015-01-12 15:40:52
---

To make sure that all the data that is being correctly formatted and received from the API, we use models. For this particular application there are 4 different models: [CaseItems](#4.1-caseitem), [Documents](#4.2-document), [Comments](#4.3-comments) and [Notes](#4.4-notes).

### 4.1 CaseItem

The `CaseItem` model is used to ensure that the correct format is received from the API. It gives structure to the view controllers of what they can expect and adds functions that can be run to fetch certain

The following attributes are present for a `CaseItem` object:

- id: Int
- title: String
- casetype: String
- status: String

##### Function: casesWithJSON(allResults: NSArray)
This function returns an `NSArray` of `CaseItem` instances.

###### Example:
```swift
  let view = UIView(frame: CGRect(x: 0, y: 0, width: 50, height: 50))
  let caseitem = CaseItem(id: 1, title: "Test case", casetype: "RFC", status: "Open")

  view.addStatusColor(caseitem)
```
