---
title: "riskyUserHistoryItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# riskyUserHistoryItem resource type




Inherits from [riskyUser](../resources/riskyUser.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get riskyUserHistoryItem](../api/riskyuserhistoryitem-get.md)|[riskyUserHistoryItem](../resources/riskyUserHistoryItem.md)|Read properties and relationships of the [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.|
|[Delete riskyUserHistoryItem](../api/riskyuserhistoryitem-delete.md)|None|Deletes a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md).|
|[Update riskyUserHistoryItem](../api/riskyuserhistoryitem-update.md)|[riskyUserHistoryItem](../resources/riskyUserHistoryItem.md)|Update the properties of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.|
|[List history](../api/riskyuserhistoryitem-list-history.md)|[riskyUserHistoryItem](../resources/riskyUserHistoryItem.md) collection|Get the riskyUserHistoryItems from the history navigation property.|
|[Add history](../api/riskyuserhistoryitem-post-history.md)|[riskyUserHistoryItem](../resources/riskyUserHistoryItem.md)|Add history by posting to the history collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|[riskUserActivity](../resources/riskUserActivity.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|initiatedBy|String||
|isDeleted|Boolean| Inherited from [riskyUser](../resources/riskyUser.md)|
|isGuest|Boolean| Inherited from [riskyUser](../resources/riskyUser.md)|
|isProcessing|Boolean| Inherited from [riskyUser](../resources/riskyUser.md)|
|riskDetail|Enumeration| Inherited from [riskyUser](../resources/riskyUser.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset| Inherited from [riskyUser](../resources/riskyUser.md)|
|riskLevel|Enumeration| Inherited from [riskyUser](../resources/riskyUser.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [riskyUser](../resources/riskyUser.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String| Inherited from [riskyUser](../resources/riskyUser.md)|
|userId|String||
|userPrincipalName|String| Inherited from [riskyUser](../resources/riskyUser.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|history|[riskyUserHistoryItem](../resources/riskyUserHistoryItem.md) collection| Inherited from [riskyUser](../resources/riskyUser.md)|

## JSON Representation
Here is a JSON representation of the resource.
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
  "isDeleted": true,
  "isGuest": true,
  "isProcessing": true,
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

