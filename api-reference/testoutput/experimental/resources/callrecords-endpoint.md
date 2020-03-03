---
title: "endpoint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph.callRecords
---


# endpoint resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|userAgent|[userAgent](../resources/callRecords-userAgent.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.endpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.endpoint",
  "userAgent": {
    "@odata.type": "microsoft.graph.callRecords.userAgent",
    "headerValue": "String",
    "applicationVersion": "String"
  }
}
```

