---
title: "SharedConnections resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# SharedConnections resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|sharedConnectionPage|String||
|topSharedConnections|[SharedConnection](../resources/sharedconnection.md) collection||
|totalCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.SharedConnections"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.SharedConnections",
  "topSharedConnections": [
    {
      "@odata.type": "microsoft.graph.SharedConnection",
      "firstName": "String",
      "lastName": "String",
      "picture": "String"
    }
  ],
  "totalCount": 1024,
  "sharedConnectionPage": "String"
}
```

