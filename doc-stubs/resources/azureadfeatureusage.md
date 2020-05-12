---
title: "azureADFeatureUsage resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# azureADFeatureUsage resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|featureName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|snapshotDateTime|DateTimeOffset|**TODO: Add Description**|
|usage|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.azureADFeatureUsage",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureADFeatureUsage",
  "id": "String (identifier)",
  "snapshotDateTime": "String (timestamp)",
  "featureName": "String",
  "usage": "Integer"
}
```

