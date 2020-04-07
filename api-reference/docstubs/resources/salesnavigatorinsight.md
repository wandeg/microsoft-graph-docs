---
title: "SalesNavigatorInsight resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# SalesNavigatorInsight resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdAt|Int64||
|detail|String||
|insightType|Enumeration| Possible values are: `IN_NETWORK`, `NEWS_MENTION`, `POST`, `PUBLISH_ARTICLE`, `SHARE_ARTICLE`, `SHARE_CONTENT`.|
|insightUrl|String||
|person|[SalesNavigatorPersonInfo](../resources/salesnavigatorpersoninfo.md)||
|photoUrl|String||
|title|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.SalesNavigatorInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.SalesNavigatorInsight",
  "createdAt": 1024,
  "insightType": "String",
  "title": "String",
  "detail": "String",
  "insightUrl": "String",
  "photoUrl": "String",
  "person": {
    "@odata.type": "microsoft.graph.SalesNavigatorPersonInfo",
    "firstName": "String",
    "lastName": "String",
    "url": "String"
  }
}
```

