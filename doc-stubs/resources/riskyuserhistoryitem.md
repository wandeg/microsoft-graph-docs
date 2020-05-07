---
title: "riskyUserHistoryItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# riskyUserHistoryItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [riskyUser](../resources/riskyuser.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List history](../api/riskyuserhistoryitem-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection|Get the riskyUserHistoryItems from the history navigation property.|
|[Create history](../api/riskyuserhistoryitem-post-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Create a new history object.|
|[Delete history](../api/riskyuserhistoryitem-delete-history.md)|None|Delete a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.|
|[Update history](../api/riskyuserhistoryitem-update-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Update the properties of a history object.|
|[Get riskyUserHistoryItem](../api/riskyuserhistoryitem-get.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.|
|[List history](../api/riskyuserhistoryitem-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection|Get the riskyUserHistoryItems from the history navigation property.|
|[Create history](../api/riskyuserhistoryitem-post-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Create a new history object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|[riskUserActivity](../resources/riskuseractivity.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|initiatedBy|String|**TODO: Add Description**|
|isDeleted|Boolean|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|isGuest|Boolean|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|isProcessing|Boolean|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|riskDetail|riskDetail|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|riskLevel|riskLevel|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|userId|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|history|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isGuest": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "initiatedBy": "String",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity"
  }
}
```

