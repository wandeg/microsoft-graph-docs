---
title: "emailFileAssessmentRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# emailFileAssessmentRequest resource type




Inherits from [threatAssessmentRequest](../resources/threatAssessmentRequest.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List emailFileAssessmentRequests](../api/emailfileassessmentrequest-list.md)|[emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md) collection|List properties and relationships of the [emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md) objects.|
|[Get emailFileAssessmentRequest](../api/emailfileassessmentrequest-get.md)|[emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md)|Read properties and relationships of the [emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md) object.|
|[Create emailFileAssessmentRequest](../api/emailfileassessmentrequest-create.md)|[emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md)|Create a new [emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md) object.|
|[Delete emailFileAssessmentRequest](../api/emailfileassessmentrequest-delete.md)|None|Deletes a [emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md).|
|[Update emailFileAssessmentRequest](../api/emailfileassessmentrequest-update.md)|[emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md)|Update the properties of a [emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md) object.|
|[List results](../api/emailfileassessmentrequest-list-results.md)|[threatAssessmentResult](../resources/threatAssessmentResult.md) collection|Get the threatAssessmentResults from the results navigation property.|
|[Add results](../api/emailfileassessmentrequest-post-results.md)|[threatAssessmentResult](../resources/threatAssessmentResult.md)|Add results by posting to the results collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md). Possible values are: `undefined`, `spam`, `phishing`, `malware`, `unknownFutureValue`.|
|contentData|String||
|contentType|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md). Possible values are: `mail`, `url`, `file`.|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md)|
|createdDateTime|DateTimeOffset| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md)|
|destinationRoutingReason|Enumeration|. Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`, `unknownFutureValue`.|
|expectedAssessment|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md). Possible values are: `block`, `unblock`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|recipientEmail|String||
|requestSource|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md). Possible values are: `undefined`, `user`, `administrator`.|
|status|Enumeration| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md). Possible values are: `pending`, `completed`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|results|[threatAssessmentResult](../resources/threatAssessmentResult.md) collection| Inherited from [threatAssessmentRequest](../resources/threatAssessmentRequest.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest",
  "baseType": "microsoft.graph.threatAssessmentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
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
  "contentData": "String"
}
```

