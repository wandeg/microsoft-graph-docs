---
title: "restrictedSignIn resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# restrictedSignIn resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [signIn](../resources/signin.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get restrictedSignIn](../api/restrictedsignin-get.md)|[restrictedSignIn](../resources/restrictedsignin.md)|Read properties and relationships of a [restrictedSignIn](../resources/restrictedsignin.md) object.|
|[Update restrictedSignIn](../api/restrictedsignin-update.md)|[restrictedSignIn](../resources/restrictedsignin.md)|Update the properties of a [restrictedSignIn](../resources/restrictedsignin.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|appId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|clientAppUsed|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|conditionalAccessStatus|conditionalAccessStatus|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|deviceDetail|[deviceDetail](../resources/devicedetail.md)|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|ipAddress|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|isInteractive|Boolean|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|location|[signInLocation](../resources/signinlocation.md)|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|resourceDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|resourceId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|riskDetail|riskDetail|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|riskEventType collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|riskLevelAggregated|riskLevel|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|riskLevel|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|status|[signInStatus](../resources/signinstatus.md)|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|targetTenantId|Guid|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|userId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|userPrincipalName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|

## Relationships
None

## JSON representation
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

