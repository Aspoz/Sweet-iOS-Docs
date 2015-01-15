---
layout: page
title: "4. Models"
category: front
date: 2015-01-12 15:40:52
---

To make sure that all the data that is being correctly formatted and received from the API, we use models. For this particular application there are 4 different models: [CaseItem](#4.1-caseitem), [Document](#4.2-document), [Comment](#4.3-comment) and [Note](#4.4-note).

### 4.1 CaseItem

The `CaseItem` model is used to give structure to what a `CaseItem` looks like.

The following attributes are present for a `CaseItem` object:

- id: Int
- title: String
- casetype: String
- status: String

##### Function: casesWithJSON( allResults: NSArray )
This function returns an `NSArray` of `CaseItem` objects.


### 4.2 Document

The `Document` model is used to give structure to what a `Document` looks like.

The following attributes are present for a `Document` object:

- id: Int
- title: String
- attachment_url: String
- updated_at: String

##### Function: documentsWithJSON( allResults: NSDictionary )
This function returns an `NSArray` of `Document` objects.



### 4.3 Comment

The `Comment` model is used to give structure to what a `Comment` looks like.

The following attributes are present for a `Document` object:

- id: Int
- body: String
- user_name: String
- created_at: String

##### Function: commentsWithJSON( allResults: NSDictionary )
This function returns an `NSArray` of `Comment` objects.



### 4.4 Note

The `Note` model is used to give structure to what a `Note` looks like.

The following attributes are present for a `Note` object:

- id: Int
- body: String
- var user_id: Int

##### Function: notesWithJSON( allResults: NSDictionary )
This function returns an `NSArray` of `Note` objects.
