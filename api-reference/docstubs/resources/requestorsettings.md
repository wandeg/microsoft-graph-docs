---
title: "requestorSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# requestorSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptRequests|Boolean|**TODO: Add Description**|
|allowedRequestors|[userSet](../resources/userset.md) collection|**TODO: Add Description**|
|scopeType|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.requestorSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.requestorSettings",
  "scopeType": "String",
  "acceptRequests": true,
  "allowedRequestors": [
    {
      "@odata.type": "microsoft.graph.singleUser",
      "isBackup": true,
      "id": "String",
      "description": "String"
    }
  ]
}
```

