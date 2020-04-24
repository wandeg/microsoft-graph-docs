---
title: "exactMatchSession resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# exactMatchSession resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [exactMatchJobBase](../resources/exactmatchjobbase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get exactMatchSession](../api/exactmatchsession-get.md)|[exactMatchSession](../resources/exactmatchsession.md)|Read the properties and relationships of an [exactMatchSession](../resources/exactmatchsession.md) object.|
|[Update exactMatchSession](../api/exactmatchsession-update.md)|[exactMatchSession](../resources/exactmatchsession.md)|Update the properties of an [exactMatchSession](../resources/exactmatchsession.md) object.|
|[cancel](../api/exactmatchsession-cancel.md)|None|**TODO: Add Description**|
|[commit](../api/exactmatchsession-commit.md)|None|**TODO: Add Description**|
|[renew](../api/exactmatchsession-renew.md)|[exactMatchSession](../resources/exactmatchsession.md)|**TODO: Add Description**|
|[List uploadAgent](../api/exactmatchsession-list-uploadagent.md)|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md) collection|Get the exactMatchUploadAgents from the uploadAgent navigation property.|
|[Create uploadAgent](../api/exactmatchsession-post-uploadagent.md)|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md)|Create a new uploadAgent object.|
|[Delete uploadAgent](../api/exactmatchsession-delete-uploadagent.md)|None|Delete an [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.|
|[Update uploadAgent](../api/exactmatchsession-update-uploadagent.md)|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md)|Update the properties of an uploadAgent object.|
|[Get exactMatchUploadAgent](../api/exactmatchuploadagent-get.md)|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md)|Read the properties and relationships of an [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|checksum|String|**TODO: Add Description**|
|completionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|creationDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|datastoreId|String|**TODO: Add Description**|
|dataUploadURI|String|**TODO: Add Description**|
|error|[classificationError](../resources/classificationerror.md)|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|fields|String collection|**TODO: Add Description**|
|fileName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|processingCompletionDateTime|DateTimeOffset|**TODO: Add Description**|
|remainingBlockCount|Int32|**TODO: Add Description**|
|remainingJobCount|Int32|**TODO: Add Description**|
|rowsPerBlock|Int32|**TODO: Add Description**|
|salt|String|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [exactMatchJobBase](../resources/exactmatchjobbase.md)|
|state|String|**TODO: Add Description**|
|totalBlockCount|Int32|**TODO: Add Description**|
|totalJobCount|Int32|**TODO: Add Description**|
|uploadAgentId|String|**TODO: Add Description**|
|uploadCompletionDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|uploadAgent|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md)|**TODO: Add Description**|

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
  "remainingJobCount": 1024,
  "salt": "String"
}
```

