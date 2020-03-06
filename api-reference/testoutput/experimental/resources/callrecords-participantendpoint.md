---
title: "participantEndpoint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# participantEndpoint resource type


Namespace: microsoft.graph.callRecords




Inherits from [endpoint](../resources/endpoint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|feedback|[userFeedback](../resources/callrecords-userfeedback.md)||
|identity|[identitySet](../resources/callrecords-identityset.md)||
|userAgent|[userAgent](../resources/callrecords-useragent.md)| Inherited from [endpoint](../resources/callrecords-endpoint.md)|

## Relationships
None

## JSON representation
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

