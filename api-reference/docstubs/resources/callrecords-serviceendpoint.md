---
title: "serviceEndpoint resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# serviceEndpoint resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**


Inherits from [endpoint](../resources/endpoint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|userAgent|[userAgent](../resources/callrecords-useragent.md)|**TODO: Add Description** Inherited from [endpoint](../resources/callrecords-endpoint.md)|

## Relationships
None

## JSON representation
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

