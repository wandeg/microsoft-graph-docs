---
title: "restrictedSignIn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# restrictedSignIn resource type




Inherits from [signIn](../resources/signIn.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List restrictedSignIns](../api/restrictedsignin-list.md)|[restrictedSignIn](../resources/restrictedSignIn.md) collection|List properties and relationships of the [restrictedSignIn](../resources/restrictedsignin.md) objects.|
|[Get restrictedSignIn](../api/restrictedsignin-get.md)|[restrictedSignIn](../resources/restrictedSignIn.md)|Read properties and relationships of the [restrictedSignIn](../resources/restrictedsignin.md) object.|
|[Create restrictedSignIn](../api/restrictedsignin-create.md)|[restrictedSignIn](../resources/restrictedSignIn.md)|Create a new [restrictedSignIn](../resources/restrictedsignin.md) object.|
|[Delete restrictedSignIn](../api/restrictedsignin-delete.md)|None|Deletes a [restrictedSignIn](../resources/restrictedsignin.md).|
|[Update restrictedSignIn](../api/restrictedsignin-update.md)|[restrictedSignIn](../resources/restrictedSignIn.md)|Update the properties of a [restrictedSignIn](../resources/restrictedsignin.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appDisplayName|String| Inherited from [signIn](../resources/signIn.md)|
|appId|String| Inherited from [signIn](../resources/signIn.md)|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedConditionalAccessPolicy.md) collection| Inherited from [signIn](../resources/signIn.md)|
|clientAppUsed|String| Inherited from [signIn](../resources/signIn.md)|
|conditionalAccessStatus|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String| Inherited from [signIn](../resources/signIn.md)|
|createdDateTime|DateTimeOffset| Inherited from [signIn](../resources/signIn.md)|
|deviceDetail|[deviceDetail](../resources/deviceDetail.md)| Inherited from [signIn](../resources/signIn.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|ipAddress|String| Inherited from [signIn](../resources/signIn.md)|
|isInteractive|Boolean| Inherited from [signIn](../resources/signIn.md)|
|location|[signInLocation](../resources/signInLocation.md)| Inherited from [signIn](../resources/signIn.md)|
|resourceDisplayName|String| Inherited from [signIn](../resources/signIn.md)|
|resourceId|String| Inherited from [signIn](../resources/signIn.md)|
|riskDetail|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection| Inherited from [signIn](../resources/signIn.md)|
|riskLevelAggregated|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|status|[signInStatus](../resources/signInStatus.md)| Inherited from [signIn](../resources/signIn.md)|
|targetTenantId|Guid||
|userDisplayName|String| Inherited from [signIn](../resources/signIn.md)|
|userId|String| Inherited from [signIn](../resources/signIn.md)|
|userPrincipalName|String| Inherited from [signIn](../resources/signIn.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedSignIn",
  "baseType": "microsoft.graph.signIn",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedSignIn",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "appId": "String",
  "appDisplayName": "String",
  "ipAddress": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "clientAppUsed": "String",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "correlationId": "String",
  "conditionalAccessStatus": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
    }
  ],
  "isInteractive": true,
  "riskDetail": "String",
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "riskEventTypes": [
    "String"
  ],
  "resourceDisplayName": "String",
  "resourceId": "String",
  "targetTenantId": "Guid"
}
```

