---
title: "participantEndpoint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph.callRecords
---


# participantEndpoint resource type




Inherits from [endpoint](../resources/endpoint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|feedback|[userFeedback](../resources/callRecords-userFeedback.md)||
|identity|[identitySet](../resources/callRecords-identitySet.md)||
|userAgent|[userAgent](../resources/callRecords-userAgent.md)| Inherited from [endpoint](../resources/callRecords-endpoint.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.participantEndpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
  "userAgent": {
    "@odata.type": "microsoft.graph.callRecords.userAgent",
    "headerValue": "String",
    "applicationVersion": "String"
  },
  "identity": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "feedback": {
    "@odata.type": "microsoft.graph.callRecords.userFeedback",
    "text": "String",
    "rating": "String",
    "tokens": {
      "@odata.type": "microsoft.graph.callRecords.feedbackTokenSet"
    }
  }
}
```

