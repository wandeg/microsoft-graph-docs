---
title: "UserGeneratedContent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# UserGeneratedContent resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdOn|[Date](../resources/date.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|mediaCategory|ShareMediaCategory|**TODO: Add Description**. Possible values are: `ARTICLE`, `IMAGE`, `NONE`, `RICH`, `VIDEO`, `LEARNING_COURSE`, `JOB`, `QUESTION`, `ANSWER`, `CAROUSEL`, `TOPIC`, `NATIVE_DOCUMENT`, `URN_REFERENCE`, `LIVE_VIDEO`.|
|thumbnails|String collection|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|url|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.UserGeneratedContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.UserGeneratedContent",
  "title": "String",
  "description": "String",
  "url": "String",
  "createdOn": {
    "@odata.type": "microsoft.graph.Date"
  },
  "thumbnails": [
    "String"
  ],
  "mediaCategory": "String"
}
```

