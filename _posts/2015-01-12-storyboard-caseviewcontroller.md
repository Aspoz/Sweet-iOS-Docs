---
layout: page
title: "7. CaseViewController"
category: story
date: 2015-01-12 16:54:00
---

### 7.1 Elements:
`Clear view logo`  
The `UIImageView` has an image which will be used in case there aren't any documents. It has a referencing outlet named 'emptyCaseViewBG' in the corresponding viewcontroller. 

`Title View`  
The Title View `UIView` is styled with the attributes inspector and can't be found in a viewcontroller.

`IN PROGRESS`  
The IN PROGRESS `UILabel` is styled with the attributes inspector and programmaticly, and has a referencing outlet named 'caseStatus' in the corresponding viewcontroller.

`NFC`  
The NFC `UILabel` is styled with the attributes inspector and programmaticly, and has a referencing outlet named 'caseType' in the corresponding viewcontroller.

`This folder is empty...`  
The `UILabel` has a text which will be used in case there aren't any documents. It has a referencing outlet named 'emptyCaseViewText' in the corresponding viewcontroller. 

'Files'
Is presenting the `UITabBarItem` which contains an image and title. It's styled in the attributes inspector.

### 7.2 Table View:
The `UITableView` has a reusable cell named 'DocumentCell' with multiple outlets. These outlets are named: 'FileBG'(`UIView`), 'PDFImage'(`UIImageView`) 'File Name'(`UILabel`), 'DateTime'(`UILabel`) and 'SeperatorLine'(`UIView`). These can be found in the corresponding instance view. The table view has the referencing outlets 'delegate', 'data source' and an outlet for itself named 'DocumentsTableView'.

### 7.3 Constraints:
Vertical Space (113), Table View to Top Layout Guide.
Horizontal Space (-16), View to This folder is empty...
Horizontal Space (-16), This folder is empty... to View.
Horizontal Space (295), Clear View Logo to View.
Horizontal Space (295), View to Clear View Logo.
Vertical Space (236), Clear View Logo to This folder is empty...
Vertical Space (391), Bottom Layout Guide to Clear View Logo.

### 7.4 Segues:

Push segue to Document View Controller (DocumentCell)
Has a relationship to 'Tab Bar Controller view controllers'

