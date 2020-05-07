---
title: "riskyUser resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# riskyUser resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List riskyUsers](../api/riskyuser-list.md)|[riskyUser](../resources/riskyuser.md) collection|Get a list of the [riskyUser](../resources/riskyuser.md) objects and their properties.|
|[Get riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|Read the properties and relationships of a [riskyUser](../resources/riskyuser.md) object.|
|[Create riskyUser](../api/riskyuser-post-riskyusers.md)|[riskyUser](../resources/riskyuser.md)|Create a new [riskyUser](../resources/riskyuser.md) object.|
|[Delete riskyUser](../api/riskyuser-delete.md)|None|Deletes a [riskyUser](../resources/riskyuser.md) object.|
|[Update riskyUser](../api/riskyuser-update.md)|[riskyUser](../resources/riskyuser.md)|Update the properties of a [riskyUser](../resources/riskyuser.md) object.|
|[dismiss](../api/riskyuser-dismiss.md)|None|**TODO: Add Description**|
|[confirmCompromised](../api/riskyuser-confirmcompromised.md)|None|**TODO: Add Description**|
|[List history](../api/riskyuser-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection|Get the riskyUserHistoryItems from the history navigation property.|
|[Create history](../api/riskyuser-post-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Create a new history object.|
|[Delete history](../api/riskyuser-delete-history.md)|None|Delete a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.|
|[Update history](../api/riskyuser-update-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Update the properties of a history object.|
|[Get riskyUserHistoryItem](../api/riskyuserhistoryitem-get.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean|**TODO: Add Description**|
|isGuest|Boolean|**TODO: Add Description**|
|isProcessing|Boolean|**TODO: Add Description**|
|riskDetail|riskDetail|**TODO: Add Description**. Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|
|riskLevel|riskLevel|**TODO: Add Description**. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|**TODO: Add Description**. Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|history|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isGuest": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```

