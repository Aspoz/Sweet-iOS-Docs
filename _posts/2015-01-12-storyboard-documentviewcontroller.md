---
layout: page
title: "9. DocumentViewController"
category: story
date: 2015-01-12 16:45:49
---

### 9.1 Elements:
`Web View`  
The `UIWebView` contains the 'documents' after they get downloaded. It's styled in the attributes inspector and programmaticly. Therefor, it has a referencing outlet named 'PdfView' in the corresponding viewcontroller.

`View`  
The `UIView` has a background for the `Text View`. It's styled in the attributes inspector. It has a referencing outlet named 'sidebar' in the corresponding viewcontroller.

`Text View`  
The Text View `UITextView` is styled with the attributes inspector and has a referencing outlet named 'noteText' in the corresponding viewcontroller.

`Add`  
The Add `UIButton` is styled with the attributes inspector. It also has an event, named 'Touch Up Inside' and is used as `IBAFunction` called 'noteSend' in the corresponding viewcontroller.

`NOTES`  
The NOTES `UIButton` is styled with the attributes inspector. It also has an event, named 'Touch Up Inside' and is used as `IBAFunction` called 'showNotes' in the corresponding viewcontroller.

`Navigation Item`  
The view controller has a forced back button.

### 9.2 Table View:
The `UITableView` has a reusable cell named 'NoteCell' with a Content View. The cells are styled in the attributes inspector. The table view has the referencing outlets 'delegate', 'data source' and an outlet for itself named 'notesView'.


