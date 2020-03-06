---
title: "recordingInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# recordingInfo resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|initiatedBy|[participantInfo](../resources/participantinfo.md)||
|recordingStatus|Enumeration|. Possible values are: `unknown`, `notRecording`, `recording`, `failed`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.recordingInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recordingInfo",
  "recordingStatus": "String",
  "initiatedBy": {
    "@odata.type": "microsoft.graph.participantInfo",
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
}
```

