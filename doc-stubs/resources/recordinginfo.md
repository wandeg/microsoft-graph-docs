---
title: "recordingInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# recordingInfo resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|initiatedBy|[participantInfo](../resources/participantinfo.md)|**TODO: Add Description**|
|initiator|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|recordingStatus|recordingStatus|**TODO: Add Description**. Possible values are: `unknown`, `notRecording`, `recording`, `failed`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.participantInfo"
  },
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

