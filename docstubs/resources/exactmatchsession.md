---
title: "exactMatchSession resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# exactMatchSession resource type


Namespace: microsoft.graph




Inherits from [exactMatchJobBase](../resources/exactmatchjobbase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get exactMatchSession](../api/exactmatchsession-get.md)|[exactMatchSession](../resources/exactmatchsession.md)|Read properties and relationships of the [exactMatchSession](../resources/exactmatchsession.md) object.|
|[Update exactMatchSession](../api/exactmatchsession-update.md)|[exactMatchSession](../resources/exactmatchsession.md)|Update the properties of a [exactMatchSession](../resources/exactmatchsession.md) object.|
|[cancel](../api/exactmatchsession-cancel.md)|None||
|[commit](../api/exactmatchsession-commit.md)|None||
|[renew](../api/exactmatchsession-renew.md)|[exactMatchSession](../resources/exactmatchsession.md)||
|[Get exactMatchUploadAgent](../api/exactmatchuploadagent-get.md)|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md)|Read properties and relationships of the [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.|
|[List sessions](../api/exactmatchdatastore-list-sessions.md)|[exactMatchSession](../resources/exactmatchsession.md) collection|Get the exactMatchSessions from the sessions navigation property.|
|[Add sessions](../api/exactmatchdatastore-post-sessions.md)|[exactMatchSession](../resources/exactmatchsession.md)|Add sessions by posting to the sessions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|checksum|String||
|completionDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|creationDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|datastoreId|String||
|dataUploadURI|String||
|error|[classificationError](../resources/classificationerror.md)| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|fields|String collection||
|fileName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdatedDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|processingCompletionDateTime|DateTimeOffset||
|remainingBlockCount|Int32||
|remainingJobCount|Int32||
|rowsPerBlock|Int32||
|startDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|state|String||
|totalBlockCount|Int32||
|totalJobCount|Int32||
|uploadAgentId|String||
|uploadCompletionDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|uploadAgent|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.exactMatchSession",
  "baseType": "microsoft.graph.exactMatchJobBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exactMatchSession",
  "id": "String (identifier)",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "String",
    "message": "String",
    "target": "String",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "String (timestamp)",
      "clientRequestId": "String",
      "activityId": "String"
    },
    "details": [
      {
        "@odata.type": "microsoft.graph.classifcationErrorBase"
      }
    ]
  },
  "datastoreId": "String",
  "uploadAgentId": "String",
  "fields": [
    "String"
  ],
  "fileName": "String",
  "checksum": "String",
  "dataUploadURI": "String",
  "remainingBlockCount": 1024,
  "totalBlockCount": 1024,
  "state": "String",
  "uploadCompletionDateTime": "String (timestamp)",
  "processingCompletionDateTime": "String (timestamp)",
  "rowsPerBlock": 1024,
  "totalJobCount": 1024,
  "remainingJobCount": 1024
}
```

