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
  endpoint_url("cases")
```

##### Returns:
```swift
  returns "http://base-url/cases"
```

### 2.2 post( endpoint: String, params: String )
Returns a `NSDictionary` with JSON data from the `POST` request. If the user is logged it, the `usertoken` will be automatically send in the request headers.

##### Example:
```swift
  post("/comments", params: "comment[body]=Erg+goed+geschreven+stuk.&comment[subject_id]=6&comment[user_id]=1")
```

##### Returns:
```swift
  {
    "id": 105,
    "user_id": 1,
    "subject_id": 6,
    "body": "Erg goed geschreven stuk.",
    "created_at": "2015-01-09T14:28:20.605Z",
    "updated_at": "2015-01-09T14:28:20.605Z"
  }
```

### 2.3 destroy( endpoint: String )
Deletes an object for the given `endpoint` as a `String`. If the user is logged it, the `usertoken` will be automatically send in the request headers.

This function **does not return anything**.

##### Example:
```swift
  destroy("/comments/5")
```

### 2.4 login( email: String, password: String )
Returns a `NSDictionary` with JSON data from the `POST` request.

##### Example:
```swift
  login("voorzitter@nam.nl", password: "Password01")
```

##### Returns:
```swift
  {
    "success": true,
    "user_id": 1,
    "group_id": 1,
    "access_token": "aea1fe91e2ba3114956a13103553df32"
  }
```

### 2.5 createUserDefaults( email: String, password: String, user: NSDictionary )
Returns a `Boolean` which sents true if the `userDefaults` were created with `email`, `password` and the complete `user` JSON.

##### Example:
```swift
  createUserDefaults("voorzitter@nam.nl", password: "Password01", user: {"success": true, "user_id": 1, "group_id": 1, "access_token": "73e1f94b84081d874f88606d7f5d9a99"})
```

##### Returns:
```swift
  true
```

### 2.6 isLoggedIn()
Returns a `Boolean`. The function checks if `isLoggedIn` is `true` in the `userDefaults`.

##### Example:
```swift
  isLoggedIn()
```

##### Returns:
```swift
  false
```

### 2.7 currentUser()
Returns a the `userid` as an `NSInteger` from the current user.

### 2.8 userToken()
Returns a `String` with the `accesstoken` from the current user.

##### Example:
```swift
  userToken()
```

##### Returns:
```swift
  "05b9283e2ad14c19d512f07db5192330"
```
