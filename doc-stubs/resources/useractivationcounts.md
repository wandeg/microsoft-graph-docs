---
title: "userActivationCounts resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userActivationCounts resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activatedOnSharedComputer|Boolean|**TODO: Add Description**|
|android|Int64|**TODO: Add Description**|
|ios|Int64|**TODO: Add Description**|
|lastActivatedDate|Date|**TODO: Add Description**|
|mac|Int64|**TODO: Add Description**|
|productType|String|**TODO: Add Description**|
|windows|Int64|**TODO: Add Description**|
|windows10Mobile|Int64|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userActivationCounts",
  "productType": "String",
  "lastActivatedDate": "Date",
  "windows": "Integer",
  "mac": "Integer",
  "windows10Mobile": "Integer",
  "ios": "Integer",
  "android": "Integer",
  "activatedOnSharedComputer": "Boolean"
}
```

