---
title: "sharingDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# sharingDetail resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|sharedBy|[insightIdentity](../resources/insightIdentity.md)||
|sharedDateTime|DateTimeOffset||
|sharingReference|[resourceReference](../resources/resourceReference.md)||
|sharingSubject|String||
|sharingType|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharingDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharingDetail",
  "sharedBy": {
    "@odata.type": "microsoft.graph.insightIdentity",
    "displayName": "String",
    "id": "String",
    "address": "String"
  },
  "sharedDateTime": "String (timestamp)",
  "sharingSubject": "String",
  "sharingType": "String",
  "sharingReference": {
    "@odata.type": "microsoft.graph.resourceReference",
    "webUrl": "String",
    "type": "String"
  }
}
```

