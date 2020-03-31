---
title: "threatAssessmentRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# threatAssessmentRequest resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get threatAssessmentRequest](../api/threatassessmentrequest-get.md)|[threatAssessmentRequest](../resources/threatassessmentrequest.md)|Read properties and relationships of the [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.|
|[List results](../api/threatassessmentrequest-list-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md) collection|Get the threatAssessmentResults from the results navigation property.|
|[Add results](../api/threatassessmentrequest-post-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md)|Add results by posting to the results collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|Enumeration| Possible values are: `undefined`, `spam`, `phishing`, `malware`, `unknownFutureValue`.|
|contentType|Enumeration| Possible values are: `mail`, `url`, `file`.|
|createdBy|[identitySet](../resources/identityset.md)||
|createdDateTime|DateTimeOffset||
|expectedAssessment|Enumeration| Possible values are: `block`, `unblock`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|requestSource|Enumeration| Possible values are: `undefined`, `user`, `administrator`.|
|status|Enumeration| Possible values are: `pending`, `completed`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|results|[threatAssessmentResult](../resources/threatassessmentresult.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.threatAssessmentRequest",
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
  }
}
```

