---
title: "mailAssessmentRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mailAssessmentRequest resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [threatAssessmentRequest](../resources/threatassessmentrequest.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List results](../api/mailassessmentrequest-list-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md) collection|Get the threatAssessmentResults from the results navigation property.|
|[Create results](../api/mailassessmentrequest-post-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md)|Create a new results object.|
|[Delete results](../api/mailassessmentrequest-delete-results.md)|None|Delete a [threatAssessmentResult](../resources/threatassessmentresult.md) object.|
|[Update results](../api/mailassessmentrequest-update-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md)|Update the properties of a results object.|
|[Get results](../api/mailassessmentrequest-get-threatassessmentresult.md)|[threatAssessmentResult](../resources/threatassessmentresult.md)|Read the properties and relationships of a [threatAssessmentResult](../resources/threatassessmentresult.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|threatCategory|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `undefined`, `spam`, `phishing`, `malware`, `unknownFutureValue`.|
|contentType|threatAssessmentContentType|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `mail`, `url`, `file`.|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md)|
|destinationRoutingReason|mailDestinationRoutingReason|**TODO: Add Description**. Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`, `unknownFutureValue`.|
|expectedAssessment|threatExpectedAssessment|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `block`, `unblock`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|messageUri|String|**TODO: Add Description**|
|recipientEmail|String|**TODO: Add Description**|
|requestSource|threatAssessmentRequestSource|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `undefined`, `user`, `administrator`.|
|status|threatAssessmentStatus|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `pending`, `completed`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|results|[threatAssessmentResult](../resources/threatassessmentresult.md) collection|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md)|

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.identitySet"
  },
  "recipientEmail": "String",
  "destinationRoutingReason": "String",
  "messageUri": "String"
}
```

