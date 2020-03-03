---
title: "fileAssessmentRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# fileAssessmentRequest resource type


Namespace: microsoft.graph




Inherits from [threatAssessmentRequest](../resources/threatassessmentrequest.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List fileAssessmentRequests](../api/fileassessmentrequest-list.md)|[fileAssessmentRequest](../resources/fileassessmentrequest.md) collection|List properties and relationships of the [fileAssessmentRequest](../resources/fileassessmentrequest.md) objects.|
|[Get fileAssessmentRequest](../api/fileassessmentrequest-get.md)|[fileAssessmentRequest](../resources/fileassessmentrequest.md)|Read properties and relationships of the [fileAssessmentRequest](../resources/fileassessmentrequest.md) object.|
|[Create fileAssessmentRequest](../api/fileassessmentrequest-create.md)|[fileAssessmentRequest](../resources/fileassessmentrequest.md)|Create a new [fileAssessmentRequest](../resources/fileassessmentrequest.md) object.|
|[Delete fileAssessmentRequest](../api/fileassessmentrequest-delete.md)|None|Deletes a [fileAssessmentRequest](../resources/fileassessmentrequest.md).|
|[Update fileAssessmentRequest](../api/fileassessmentrequest-update.md)|[fileAssessmentRequest](../resources/fileassessmentrequest.md)|Update the properties of a [fileAssessmentRequest](../resources/fileassessmentrequest.md) object.|
|[List results](../api/fileassessmentrequest-list-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md) collection|Get the threatAssessmentResults from the results navigation property.|
|[Add results](../api/fileassessmentrequest-post-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md)|Add results by posting to the results collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `undefined`, `spam`, `phishing`, `malware`, `unknownFutureValue`.|
|contentData|String||
|contentType|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `mail`, `url`, `file`.|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md)|
|createdDateTime|DateTimeOffset| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md)|
|expectedAssessment|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `block`, `unblock`.|
|fileName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|requestSource|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `undefined`, `user`, `administrator`.|
|status|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `pending`, `completed`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|results|[threatAssessmentResult](../resources/threatassessmentresult.md) collection| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fileAssessmentRequest",
  "baseType": "microsoft.graph.threatAssessmentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileAssessmentRequest",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "contentType": "String",
  "expectedAssessment": "String",
  "category": "String",
  "status": "String",
  "requestSource": "String",
  "createdBy": {
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
  "fileName": "String",
  "contentData": "String"
}
```

