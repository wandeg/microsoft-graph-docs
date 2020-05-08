---
title: "participantEndpoint resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# participantEndpoint resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**


Inherits from [endpoint](../resources/endpoint.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|feedback|[userFeedback](../resources/callrecords-userfeedback.md)|**TODO: Add Description**|
|identity|[identitySet](../resources/callrecords-identityset.md)|**TODO: Add Description**|
|userAgent|[userAgent](../resources/callrecords-useragent.md)|**TODO: Add Description** Inherited from [endpoint](../resources/callrecords-endpoint.md)|

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
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "application": {
      "@odata.type": "microsoft.graph.identity"
    },
    "device": {
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

