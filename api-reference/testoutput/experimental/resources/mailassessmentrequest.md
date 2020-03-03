---
title: "mailAssessmentRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mailAssessmentRequest resource type


Namespace: microsoft.graph




Inherits from [threatAssessmentRequest](../resources/threatassessmentrequest.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mailAssessmentRequests](../api/mailassessmentrequest-list.md)|[mailAssessmentRequest](../resources/mailassessmentrequest.md) collection|List properties and relationships of the [mailAssessmentRequest](../resources/mailassessmentrequest.md) objects.|
|[Get mailAssessmentRequest](../api/mailassessmentrequest-get.md)|[mailAssessmentRequest](../resources/mailassessmentrequest.md)|Read properties and relationships of the [mailAssessmentRequest](../resources/mailassessmentrequest.md) object.|
|[Create mailAssessmentRequest](../api/mailassessmentrequest-create.md)|[mailAssessmentRequest](../resources/mailassessmentrequest.md)|Create a new [mailAssessmentRequest](../resources/mailassessmentrequest.md) object.|
|[Delete mailAssessmentRequest](../api/mailassessmentrequest-delete.md)|None|Deletes a [mailAssessmentRequest](../resources/mailassessmentrequest.md).|
|[Update mailAssessmentRequest](../api/mailassessmentrequest-update.md)|[mailAssessmentRequest](../resources/mailassessmentrequest.md)|Update the properties of a [mailAssessmentRequest](../resources/mailassessmentrequest.md) object.|
|[List results](../api/mailassessmentrequest-list-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md) collection|Get the threatAssessmentResults from the results navigation property.|
|[Add results](../api/mailassessmentrequest-post-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md)|Add results by posting to the results collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `undefined`, `spam`, `phishing`, `malware`, `unknownFutureValue`.|
|contentType|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `mail`, `url`, `file`.|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md)|
|createdDateTime|DateTimeOffset| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md)|
|destinationRoutingReason|Enumeration|. Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`, `unknownFutureValue`.|
|expectedAssessment|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `block`, `unblock`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|messageUri|String||
|recipientEmail|String||
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
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "baseType": "microsoft.graph.threatAssessmentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailAssessmentRequest",
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
  "recipientEmail": "String",
  "destinationRoutingReason": "String",
  "messageUri": "String"
}
```

