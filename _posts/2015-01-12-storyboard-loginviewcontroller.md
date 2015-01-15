---
layout: page
title: "3. LoginViewController"
category: story
date: 2015-01-12 16:58:00
---
Is the Initial View Controller.

### 3.1 Elements:
`Email`  
The Email `UITextField` is styled with the attributes inspector and has a referencing outlet named 'txtUsername' in the corresponding viewcontroller.

`Password`  
The Password `UITextField` is styled with the attributes inspector and has a referencing outlet named 'txtPassword' in the corresponding viewcontroller.

`LOG IN`  
The LOG IN `UIButton` is styled with the attributes inspector and in his viewcontroller and has a referencing outlet named 'loginButton' in the corresponding viewcontroller. It also has an event, named 'Touch Up Inside' and is used as `IBAFunction` called 'signinTapped' in the corresponding viewcontroller.

### 3.2 Segues:

Modal segue with identifier 'loginSuccess' to Navigation Controller (LOG IN `UIButton`).
