---
layout: page
title: "3. Functions"
category: back
date: 2015-01-12 16:27:36
---

All the child controllers from `class Backend` have access to the following functions:

### 2.1 endpoint_url( param: String )
Returns a `NS_URL` with the API URL for the given `param`.

##### Example:
```swift

endpoint_url("foo")
// returns 'http://base-url/foo'


```

