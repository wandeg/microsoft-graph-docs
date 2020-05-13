---
title: "Position resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# Position resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|location|String|**TODO: Add Description**|
|logo|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|startEndDate|[DateRange](../resources/daterange.md)|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|url|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.Position"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.Position",
  "name": "String",
  "logo": "String",
  "url": "String",
  "location": "String",
  "title": "String",
  "startEndDate": {
    "@odata.type": "microsoft.graph.DateRange"
  },
  "description": "String"
}
```

