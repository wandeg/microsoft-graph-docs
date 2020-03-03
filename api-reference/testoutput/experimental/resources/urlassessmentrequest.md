---
title: "urlAssessmentRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# urlAssessmentRequest resource type




Inherits from [threatAssessmentRequest](../resources/threatAssessmentRequest.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List urlAssessmentRequests](../api/urlassessmentrequest-list.md)|[urlAssessmentRequest](../resources/urlAssessmentRequest.md) collection|List properties and relationships of the [urlAssessmentRequest](../resources/urlassessmentrequest.md) objects.|
|[Get urlAssessmentRequest](../api/urlassessmentrequest-get.md)|[urlAssessmentRequest](../resources/urlAssessmentRequest.md)|Read properties and relationships of the [urlAssessmentRequest](../resources/urlassessmentrequest.md) object.|
|[Create urlAssessmentRequest](../api/urlassessmentrequest-create.md)|[urlAssessmentRequest](../resources/urlAssessmentRequest.md)|Create a new [urlAssessmentRequest](../resources/urlassessmentrequest.md) object.|
|[Delete urlAssessmentRequest](../api/urlassessmentrequest-delete.md)|None|Deletes a [urlAssessmentRequest](../resources/urlassessmentrequest.md).|
|[Update urlAssessmentRequest](../api/urlassessmentrequest-update.md)|[urlAssessmentRequest](../resources/urlAssessmentRequest.md)|Update the properties of a [urlAssessmentRequest](../resources/urlassessmentrequest.md) object.|
|[List results](../api/urlassessmentrequest-list-results.md)|[threatAssessmentResult](../resources/threatAssessmentResult.md) collection|Get the threatAssessmentResults from the results navigation property.|
|[Add results](../api/urlassessmentrequest-post-results.md)|[threatAssessmentResult](../resources/threatAssessmentResult.md)|Add results by posting to the results collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md). Possible values are: `undefined`, `spam`, `phishing`, `malware`, `unknownFutureValue`.|
|contentType|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md). Possible values are: `mail`, `url`, `file`.|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md)|
|createdDateTime|DateTimeOffset| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md)|
|expectedAssessment|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md). Possible values are: `block`, `unblock`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|requestSource|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md). Possible values are: `undefined`, `user`, `administrator`.|
|status|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md). Possible values are: `pending`, `completed`.|
|url|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|results|[threatAssessmentResult](../resources/threatAssessmentResult.md) collection| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.urlAssessmentRequest",
  "baseType": "microsoft.graph.threatAssessmentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.urlAssessmentRequest",
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
  "url": "String"
}
```

