---
title: "riskyUserHistoryItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# riskyUserHistoryItem resource type


Namespace: microsoft.graph




Inherits from [riskyUser](../resources/riskyuser.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List riskyUserHistoryItems](../api/riskyuserhistoryitem-list.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection|List properties and relationships of the [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) objects.|
|[Get riskyUserHistoryItem](../api/riskyuserhistoryitem-get.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Read properties and relationships of the [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.|
|[Create riskyUserHistoryItem](../api/riskyuserhistoryitem-create.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Create a new [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.|
|[Delete riskyUserHistoryItem](../api/riskyuserhistoryitem-delete.md)|None|Deletes a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md).|
|[Update riskyUserHistoryItem](../api/riskyuserhistoryitem-update.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Update the properties of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.|
|[List history](../api/riskyuserhistoryitem-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection|Get the riskyUserHistoryItems from the history navigation property.|
|[Add history](../api/riskyuserhistoryitem-post-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Add history by posting to the history collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|[riskUserActivity](../resources/riskuseractivity.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|initiatedBy|String||
|isDeleted|Boolean| Inherited from [riskyUser](../resources/riskyuser.md)|
|isGuest|Boolean| Inherited from [riskyUser](../resources/riskyuser.md)|
|isProcessing|Boolean| Inherited from [riskyUser](../resources/riskyuser.md)|
|riskDetail|Enumeration| Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset| Inherited from [riskyUser](../resources/riskyuser.md)|
|riskLevel|Enumeration| Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String| Inherited from [riskyUser](../resources/riskyuser.md)|
|userId|String||
|userPrincipalName|String| Inherited from [riskyUser](../resources/riskyuser.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|history|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection| Inherited from [riskyUser](../resources/riskyuser.md)|

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

