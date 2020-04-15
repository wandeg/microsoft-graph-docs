---
title: "restrictedSignIn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# restrictedSignIn resource type


Namespace: Microsoft.AAD.Reporting




Inherits from [signIn](../resources/signin.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get restrictedSignIn](../api/microsoft.aad.reporting-restrictedsignin-get.md)|[restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md)|Read properties and relationships of the [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) object.|
|[Update restrictedSignIn](../api/microsoft.aad.reporting-restrictedsignin-update.md)|[restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md)|Update the properties of a [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alternateSignInName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|appDisplayName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|appId|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/microsoft.aad.reporting-appliedconditionalaccesspolicy.md) collection| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|authenticationDetails|[authenticationDetail](../resources/microsoft.aad.reporting-authenticationdetail.md) collection| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|authenticationMethodsUsed|String collection| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|authenticationProcessingDetails|[keyValue](../resources/microsoft.aad.reporting-keyvalue.md) collection| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/microsoft.aad.reporting-authenticationrequirementpolicy.md) collection| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|clientAppUsed|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|conditionalAccessStatus|Enumeration| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|createdDateTime|DateTimeOffset| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|deviceDetail|[deviceDetail](../resources/microsoft.aad.reporting-devicedetail.md)| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|id|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|ipAddress|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|isInteractive|Boolean| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|location|[signInLocation](../resources/microsoft.aad.reporting-signinlocation.md)| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|mfaDetail|[mfaDetail](../resources/microsoft.aad.reporting-mfadetail.md)| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|networkLocationDetails|[networkLocationDetail](../resources/microsoft.aad.reporting-networklocationdetail.md) collection| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|originalRequestId|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|processingTimeInMilliseconds|Int32| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|resourceDisplayName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|resourceId|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|riskDetail|Enumeration| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|riskLevelAggregated|Enumeration| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|servicePrincipalId|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|servicePrincipalName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|status|[signInStatus](../resources/microsoft.aad.reporting-signinstatus.md)| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|targetTenantId|Guid||
|tokenIssuerName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|tokenIssuerType|Enumeration| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userDisplayName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userId|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userPrincipalName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.AAD.Reporting.restrictedSignIn",
  "baseType": "Microsoft.AAD.Reporting.signIn",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.restrictedSignIn",
  "alternateSignInName": "String",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.appliedConditionalAccessPolicy"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.authenticationDetail"
    }
  ],
  "authenticationMethodsUsed": [
    "String"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.keyValue"
    }
  ],
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.authenticationRequirementPolicy"
    }
  ],
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "deviceDetail": {
    "@odata.type": "Microsoft.AAD.Reporting.deviceDetail"
  },
  "id": "String (identifier)",
  "isInteractive": true,
  "ipAddress": "String",
  "location": {
    "@odata.type": "Microsoft.AAD.Reporting.signInLocation"
  },
  "mfaDetail": {
    "@odata.type": "Microsoft.AAD.Reporting.mfaDetail"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.networkLocationDetail"
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
    "@odata.type": "Microsoft.AAD.Reporting.signInStatus"
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

