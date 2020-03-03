---
title: "endpoint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# endpoint resource type


Namespace: microsoft.graph.callRecords



## Properties
|Property|Type|Description|
|:---|:---|:---|
|userAgent|[userAgent](../resources/callrecords-useragent.md)||

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

