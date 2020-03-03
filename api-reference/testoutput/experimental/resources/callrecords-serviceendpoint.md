---
title: "serviceEndpoint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph.callRecords
---


# serviceEndpoint resource type




Inherits from [endpoint](../resources/endpoint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|userAgent|[userAgent](../resources/callRecords-userAgent.md)| Inherited from [endpoint](../resources/callRecords-endpoint.md)|

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

