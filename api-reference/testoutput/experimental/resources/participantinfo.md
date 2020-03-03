---
title: "participantInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# participantInfo resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|countryCode|String||
|endpointType|Enumeration|. Possible values are: `default`, `voicemail`, `skypeForBusiness`, `skypeForBusinessVoipPhone`, `unknownFutureValue`.|
|identity|[identitySet](../resources/identitySet.md)||
|languageId|String||
|region|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.participantInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.participantInfo",
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
  "endpointType": "String",
  "region": "String",
  "languageId": "String",
  "countryCode": "String"
}
```

