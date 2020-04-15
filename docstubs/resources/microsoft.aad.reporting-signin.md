---
title: "signIn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# signIn resource type


Namespace: Microsoft.AAD.Reporting



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get signIn](../api/microsoft.aad.reporting-signin-get.md)|[signIn](../resources/microsoft.aad.reporting-signin.md)|Read properties and relationships of the [signIn](../resources/microsoft.aad.reporting-signin.md) object.|
|[Update signIn](../api/microsoft.aad.reporting-signin-update.md)|[signIn](../resources/microsoft.aad.reporting-signin.md)|Update the properties of a [signIn](../resources/microsoft.aad.reporting-signin.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alternateSignInName|String||
|appDisplayName|String||
|appId|String||
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/microsoft.aad.reporting-appliedconditionalaccesspolicy.md) collection||
|authenticationDetails|[authenticationDetail](../resources/microsoft.aad.reporting-authenticationdetail.md) collection||
|authenticationMethodsUsed|String collection||
|authenticationProcessingDetails|[keyValue](../resources/microsoft.aad.reporting-keyvalue.md) collection||
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/microsoft.aad.reporting-authenticationrequirementpolicy.md) collection||
|clientAppUsed|String||
|conditionalAccessStatus|Enumeration| Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String||
|createdDateTime|DateTimeOffset||
|deviceDetail|[deviceDetail](../resources/microsoft.aad.reporting-devicedetail.md)||
|id|String||
|ipAddress|String||
|isInteractive|Boolean||
|location|[signInLocation](../resources/microsoft.aad.reporting-signinlocation.md)||
|mfaDetail|[mfaDetail](../resources/microsoft.aad.reporting-mfadetail.md)||
|networkLocationDetails|[networkLocationDetail](../resources/microsoft.aad.reporting-networklocationdetail.md) collection||
|originalRequestId|String||
|processingTimeInMilliseconds|Int32||
|resourceDisplayName|String||
|resourceId|String||
|riskDetail|Enumeration| Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection||
|riskLevelAggregated|Enumeration| Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration| Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|servicePrincipalId|String||
|servicePrincipalName|String||
|status|[signInStatus](../resources/microsoft.aad.reporting-signinstatus.md)||
|tokenIssuerName|String||
|tokenIssuerType|Enumeration| Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String||
|userDisplayName|String||
|userId|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.AAD.Reporting.signIn",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.signIn",
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
  "userPrincipalName": "String"
}
```

