---
title: "detectedSensitiveContentBase resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# detectedSensitiveContentBase resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|confidence|Int32|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|Guid|**TODO: Add Description**|
|matches|[sensitiveContentLocation](../resources/sensitivecontentlocation.md) collection|**TODO: Add Description**|
|recommendedConfidence|Int32|**TODO: Add Description**|
|uniqueCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.detectedSensitiveContentBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedSensitiveContentBase",
  "id": "String (identifier)",
  "displayName": "String",
  "uniqueCount": "Integer",
  "confidence": "Integer",
  "recommendedConfidence": "Integer",
  "matches": [
    {
      "@odata.type": "microsoft.graph.sensitiveContentLocation"
    }
  ]
}
```

