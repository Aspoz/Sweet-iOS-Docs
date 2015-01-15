---
layout: page
title: "5. OverviewViewController"
category: story
date: 2015-01-12 16:56:00
---

### 5.1 Elements:
`All, RFC, NFI, RFA, info`  
The `UISegmentedControl` has five buttons and is styled with the attributes inspector and in his viewcontroller. It has a referencing outlet named 'filterControl' in the corresponding viewcontroller. It also has a 'sent event' named 'value changed' and is called 'filter' in the corresponding viewcontroller.

`Status Color`  
The Status color `UIView` is styled programmaticly and has a referencing outlet named 'inProgressStatusControl' in the corresponding viewcontroller.

`IN PROGRESS`  
The IN PROGRESS `UILabel` is styled with the attributes inspector and can't be found in a viewcontroller.

`Status Color`  
The Status color `UIView` is styled programmaticly and has a referencing outlet named 'openStatusControl' in the corresponding viewcontroller.

`OPEN`  
The OPEN `UILabel` is styled with the attributes inspector and can't be found in a viewcontroller.

`Status Color`  
The Status color `UIView` is styled programmaticly and has a referencing outlet named 'closedStatusControl' in the corresponding viewcontroller.

`CLOSED`  
The CLOSED `UILabel` is styled with the attributes inspector and can't be found in a viewcontroller.

`LOG IN`  
The LOG IN `UIButton` is styled with the attributes inspector and in his viewcontroller and has a referencing outlet named 'loginButton' in the corresponding viewcontroller. It also has an event, named 'Touch Up Inside' and is used as `IBAFunction` called 'signinTapped' in the corresponding viewcontroller.

### 5.2 Table View:
The `UITableView` has a reusable cell named 'OverviewCell' with multiple outlets. These outlets are named: 'CaseBG'(`UIView`), 'CaseStatusColor'(`UIView`), 'CaseTitle'(`UILabel`) and 'CaseType'(`UILabel`). These can be found in the corresponding instance view. The table view has the referencing outlets 'delegate', 'data source' and an outlet for itself named 'OverviewTableView'.

### 5.3 Constraints:
Vertical space - (125) - table view - view.

### 5.4 Segues:

Modal segue to LoginViewController (log out button)
Push segue to Tab Bar Controller (OverviewCell)
Has a relationship 'root view controller' to OverviewViewController
