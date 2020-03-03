---
title: "serviceEndpoint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# serviceEndpoint resource type


Namespace: microsoft.graph.callRecords




Inherits from [endpoint](../resources/endpoint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|userAgent|[userAgent](../resources/callrecords-useragent.md)| Inherited from [endpoint](../resources/callrecords-endpoint.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.serviceEndpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.serviceEndpoint",
  "userAgent": {
    "@odata.type": "microsoft.graph.callRecords.userAgent",
    "headerValue": "String",
    "applicationVersion": "String"
  }
}
```

