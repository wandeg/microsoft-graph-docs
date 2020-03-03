---
title: "signIn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# signIn resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List signIns](../api/signin-list.md)|[signIn](../resources/signin.md) collection|List properties and relationships of the [signIn](../resources/signin.md) objects.|
|[Get signIn](../api/signin-get.md)|[signIn](../resources/signin.md)|Read properties and relationships of the [signIn](../resources/signin.md) object.|
|[Create signIn](../api/signin-create.md)|[signIn](../resources/signin.md)|Create a new [signIn](../resources/signin.md) object.|
|[Delete signIn](../api/signin-delete.md)|None|Deletes a [signIn](../resources/signin.md).|
|[Update signIn](../api/signin-update.md)|[signIn](../resources/signin.md)|Update the properties of a [signIn](../resources/signin.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alternateSignInName|String||
|appDisplayName|String||
|appId|String||
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection||
|authenticationDetails|[authenticationDetail](../resources/authenticationdetail.md) collection||
|authenticationMethodsUsed|String collection||
|authenticationProcessingDetails|[keyValue](../resources/keyvalue.md) collection||
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md) collection||
|clientAppUsed|String||
|conditionalAccessStatus|Enumeration|. Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String||
|createdDateTime|DateTimeOffset||
|deviceDetail|[deviceDetail](../resources/devicedetail.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|ipAddress|String||
|isInteractive|Boolean||
|location|[signInLocation](../resources/signinlocation.md)||
|mfaDetail|[mfaDetail](../resources/mfadetail.md)||
|networkLocationDetails|[networkLocationDetail](../resources/networklocationdetail.md) collection||
|originalRequestId|String||
|processingTimeInMilliseconds|Int32||
|resourceDisplayName|String||
|resourceId|String||
|riskDetail|Enumeration|. Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection||
|riskLevelAggregated|Enumeration|. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration|. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration|. Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|servicePrincipalId|String||
|servicePrincipalName|String||
|status|[signInStatus](../resources/signinstatus.md)||
|tokenIssuerName|String||
|tokenIssuerType|Enumeration|. Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String||
|userDisplayName|String||
|userId|String||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.signIn",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.signIn",
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
  "userPrincipalName": "String"
}
```

