---
title: "riskyUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# riskyUser resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List riskyUsers](../api/riskyuser-list.md)|[riskyUser](../resources/riskyuser.md) collection|List properties and relationships of the [riskyUser](../resources/riskyuser.md) objects.|
|[Get riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|Read properties and relationships of the [riskyUser](../resources/riskyuser.md) object.|
|[Create riskyUser](../api/riskyuser-post-riskyusers.md)|[riskyUser](../resources/riskyuser.md)|Create a new [riskyUser](../resources/riskyuser.md) object.|
|[Delete riskyUser](../api/riskyuser-delete.md)|None|Deletes a [riskyUser](../resources/riskyuser.md).|
|[Update riskyUser](../api/riskyuser-update.md)|[riskyUser](../resources/riskyuser.md)|Update the properties of a [riskyUser](../resources/riskyuser.md) object.|
|[dismiss](../api/riskyuser-dismiss.md)|None||
|[confirmCompromised](../api/riskyuser-confirmcompromised.md)|None||
|[List history](../api/riskyuser-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection|Get the riskyUserHistoryItems from the history navigation property.|
|[Add history](../api/riskyuser-post-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Add history by posting to the history collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|isGuest|Boolean||
|isProcessing|Boolean||
|riskDetail|Enumeration|. Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset||
|riskLevel|Enumeration|. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration|. Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String||
|userPrincipalName|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|history|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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
  "isDeleted": true,
  "isGuest": true,
  "isProcessing": true,
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```

