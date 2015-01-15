---
layout: page
title: "5. DictionaryController"
category: back
date: 2015-01-12 10:43:03
---

The `class DictController` can use the following functions:

### 5.1 DictControllerProtocol
Protocol which makes sure `func didReceiveAPIResults`'s result is a NSDictionary.

##### Example:
You can find an init of the DictControllerProtocol in various viewControllers.

### 5.2 Variables
```swift
var delegate: DictControllerProtocol
```
Defines type of variable 'delegate', which is a Protocol.

```swift
var backend = Backend()
```
Defines 'backend' as variable for the class [Backend](../back/backend-introduction.html).

### 5.3 get(path: String, getSuccess: () -> Void)
Uses Backend.BASE_URL + path to obtain a full url to get a dictionary. This url is used in the request which the function does. It get's a dictionary with json items and will send to `self.delegate.didReceiveAPIResults(jsonResult)`.

##### Example of the json result:
```swift
{
    id: 33,
    title: "Platform Driller Specificaties",
    created_at: "2014-11-24T11:24:41.746Z",
    updated_at: "2014-11-24T11:24:41.746Z",
    attachment_file_name: "Platform_Driller_Specificaties.pdf",
    attachment_content_type: "application/pdf",
    attachment_url: "178.62.204.157/system/attachments/000/000/033/     original/Platform_Driller_Specificaties.pdf",
    _links: {
        notes: [
            {
                id: 99,
                body: "Dit paragraaf moet vera...",
                "created_at": "2014-12-08T21:50:09.828Z",
                "updated_at": "2014-12-08T21:50:09.828Z",
                user_id: 2
            }
        ]
    }
}
```

### 5.4 caseUrl(id: Int, success: () -> Void)
Builds an url out of base url + "/cases\(id)".
Is the callback function of the get function.

### 5.5 notesUrl(id: Int, success: () -> Void)
Builds an url out of base url + "/notes\(id)".
Is the callback function of the get function.

