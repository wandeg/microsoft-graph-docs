---
title: "requestorSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# requestorSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptRequests|Boolean||
|allowedRequestors|[userSet](../resources/userset.md) collection||
|scopeType|String||

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

