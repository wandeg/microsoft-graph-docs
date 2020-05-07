---
title: "SalesNavigatorInsight resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# SalesNavigatorInsight resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdAt|Int64|**TODO: Add Description**|
|detail|String|**TODO: Add Description**|
|insightType|SalesNavigatorInsightType|**TODO: Add Description**. Possible values are: `IN_NETWORK`, `NEWS_MENTION`, `POST`, `PUBLISH_ARTICLE`, `SHARE_ARTICLE`, `SHARE_CONTENT`.|
|insightUrl|String|**TODO: Add Description**|
|person|[SalesNavigatorPersonInfo](../resources/salesnavigatorpersoninfo.md)|**TODO: Add Description**|
|photoUrl|String|**TODO: Add Description**|
|title|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.SalesNavigatorInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.SalesNavigatorInsight",
  "createdAt": "Integer",
  "insightType": "String",
  "title": "String",
  "detail": "String",
  "insightUrl": "String",
  "photoUrl": "String",
  "person": {
    "@odata.type": "microsoft.graph.SalesNavigatorPersonInfo"
  }
}
```

