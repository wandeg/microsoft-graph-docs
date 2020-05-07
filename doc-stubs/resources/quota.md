---
title: "quota resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# quota resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deleted|Int64|**TODO: Add Description**|
|remaining|Int64|**TODO: Add Description**|
|state|String|**TODO: Add Description**|
|storagePlanInformation|[storagePlanInformation](../resources/storageplaninformation.md)|**TODO: Add Description**|
|total|Int64|**TODO: Add Description**|
|used|Int64|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.quota"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.quota",
  "deleted": "Integer",
  "remaining": "Integer",
  "state": "String",
  "total": "Integer",
  "used": "Integer",
  "storagePlanInformation": {
    "@odata.type": "microsoft.graph.storagePlanInformation"
  }
}
```

