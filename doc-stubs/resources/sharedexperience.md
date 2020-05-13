---
title: "SharedExperience resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# SharedExperience resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|location|String|**TODO: Add Description**|
|logo|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|overlapInfo|[OverlapInfo](../resources/overlapinfo.md)|**TODO: Add Description**|
|url|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.SharedExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.SharedExperience",
  "name": "String",
  "logo": "String",
  "url": "String",
  "location": "String",
  "overlapInfo": {
    "@odata.type": "microsoft.graph.OverlapInfo"
  }
}
```

