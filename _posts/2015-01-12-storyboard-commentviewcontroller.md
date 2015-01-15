---
layout: page
title: "8. CommentViewController"
category: story
date: 2015-01-12 16:53:00
---

### 8.1 Elements:
`View`  
The `UIView` has a background for the `Text View`. It's styled in the attributes inspector.

`Text View`  
The Text View `UITextView` is styled with the attributes inspector and has a referencing outlet named 'commentText' in the corresponding viewcontroller.

`Add`  
The Add `UIButton` is styled with the attributes inspector. It also has an event, named 'Touch Up Inside' and is used as `IBAFunction` called 'commentSend' in the corresponding viewcontroller.

'Comments'
Is presenting the `UITabBarItem` which contains an image and title. It's styled in the attributes inspector.

### 8.2 Table View:
The `UITableView` has a reusable cell named 'CommentCell' with multiple outlets. These outlets are named: 'CommentAuthor'(`UILabel`), 'CommentBody'(`UILabel`) and 'CommentDate'(`UILabel`). These can be found in the corresponding instance view. The table view has the referencing outlets 'delegate', 'data source' and an outlet for itself named 'commentTableView'.

### 8.3 Constraints:
Horizontal Space - (7) - Label - Content View
Vertical Space - (7) - Label - Content View
Vertical Space - (1) - Content View - Label
Vertical Space - (27) - Label - Content View
Leading Alignment - Label - Label
Horizontal Space - Label - Label
Horizontal Space - (15) - Content View - Label
Vertical Space - (5) - Label - Content View
Horizontal Space - (69) - Label - Label
Vertical Space - (16) - Content View - Label

### 8.4 Segues:

Has a relationship to 'Tab Bar Controller view controllers'




