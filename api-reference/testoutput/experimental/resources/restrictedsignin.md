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
|alternateSignInName|String| Inherited from [signIn](../resources/signIn.md)|
|appDisplayName|String| Inherited from [signIn](../resources/signIn.md)|
|appId|String| Inherited from [signIn](../resources/signIn.md)|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedConditionalAccessPolicy.md) collection| Inherited from [signIn](../resources/signIn.md)|
|authenticationDetails|[authenticationDetail](../resources/authenticationDetail.md) collection| Inherited from [signIn](../resources/signIn.md)|
|authenticationMethodsUsed|String collection| Inherited from [signIn](../resources/signIn.md)|
|authenticationProcessingDetails|[keyValue](../resources/keyValue.md) collection| Inherited from [signIn](../resources/signIn.md)|
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/authenticationRequirementPolicy.md) collection| Inherited from [signIn](../resources/signIn.md)|
|clientAppUsed|String| Inherited from [signIn](../resources/signIn.md)|
|conditionalAccessStatus|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String| Inherited from [signIn](../resources/signIn.md)|
|createdDateTime|DateTimeOffset| Inherited from [signIn](../resources/signIn.md)|
|deviceDetail|[deviceDetail](../resources/deviceDetail.md)| Inherited from [signIn](../resources/signIn.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|ipAddress|String| Inherited from [signIn](../resources/signIn.md)|
|isInteractive|Boolean| Inherited from [signIn](../resources/signIn.md)|
|location|[signInLocation](../resources/signInLocation.md)| Inherited from [signIn](../resources/signIn.md)|
|mfaDetail|[mfaDetail](../resources/mfaDetail.md)| Inherited from [signIn](../resources/signIn.md)|
|networkLocationDetails|[networkLocationDetail](../resources/networkLocationDetail.md) collection| Inherited from [signIn](../resources/signIn.md)|
|originalRequestId|String| Inherited from [signIn](../resources/signIn.md)|
|processingTimeInMilliseconds|Int32| Inherited from [signIn](../resources/signIn.md)|
|resourceDisplayName|String| Inherited from [signIn](../resources/signIn.md)|
|resourceId|String| Inherited from [signIn](../resources/signIn.md)|
|riskDetail|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection| Inherited from [signIn](../resources/signIn.md)|
|riskLevelAggregated|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|servicePrincipalId|String| Inherited from [signIn](../resources/signIn.md)|
|servicePrincipalName|String| Inherited from [signIn](../resources/signIn.md)|
|status|[signInStatus](../resources/signInStatus.md)| Inherited from [signIn](../resources/signIn.md)|
|targetTenantId|Guid||
|tokenIssuerName|String| Inherited from [signIn](../resources/signIn.md)|
|tokenIssuerType|Enumeration| Inherited from [signIn](../resources/signIn.md). Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String| Inherited from [signIn](../resources/signIn.md)|
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
  "alternateSignInName": "String",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "microsoft.graph.authenticationDetail"
    }
  ],
  "authenticationMethodsUsed": [
    "String"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ],
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
    }
  ],
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "isInteractive": true,
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail"
    }
  ],
  "originalRequestId": "String",
  "processingTimeInMilliseconds": 1024,
  "riskDetail": "String",
  "riskEventTypes": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "String",
  "resourceId": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "targetTenantId": "Guid"
}
```

