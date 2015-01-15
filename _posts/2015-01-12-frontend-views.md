---
layout: page
title: "3. Views"
category: front
date: 2015-01-12 16:36:08
---

Views provide code which is mostly used for the design of 'partials' such as table cells and buttons. Outlets are called and get an improved design based of code in the views. It can be use for recurring elements.

### 3.1 LoadingSpinner
The `class LoadingSpinner` being used to instantiate a loading spinner while a certain action is going on. It has two functions called: `startLoadingSpinner(view: UIView)` and `stopLoadingSpinner()`. These functions do not return anyting.

##### Example:
```swift

  class ExampleViewController: ApplicationViewController {
    let spinner = LoadingSpinner()

    override func viewDidLoad() {
      spinner.startLoadingSpinner(view)
    }

    func ifAPICallIsDoneLoading() {
      spinner.stopLoadingSpinner()
    }
  }
```



### 3.2 StatusColor
The `class StatusColor` being used add a templating format for an `UIView` to give a case an status color. It will make the UIView round using the `roundedCorners extension`.

##### Dependence:
Requires the `makeRound()` extensions.
