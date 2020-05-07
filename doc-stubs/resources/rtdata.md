---
title: "RTData resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# RTData resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attribute|[RTAttribute](../resources/rtattribute.md) collection|**TODO: Add Description**|
|endIdx|Int32|**TODO: Add Description**|
|startIdx|Int32|**TODO: Add Description**|
|type|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.RTData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.RTData",
  "type": "String",
  "startIdx": "Integer",
  "endIdx": "Integer",
  "attribute": [
    {
      "@odata.type": "microsoft.graph.RTAttribute"
    }
  ]
}
```

