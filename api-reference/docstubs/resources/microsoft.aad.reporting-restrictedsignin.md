---
title: "restrictedSignIn resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# restrictedSignIn resource type


Namespace: Microsoft.AAD.Reporting

**TODO: Add Description**


Inherits from [signIn](../resources/signin.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get restrictedSignIn](../api/microsoft.aad.reporting-restrictedsignin-get.md)|[restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md)|Read properties and relationships of a [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) object.|
|[Update restrictedSignIn](../api/microsoft.aad.reporting-restrictedsignin-update.md)|[restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md)|Update the properties of a [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|alternateSignInName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|appDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|appId|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/microsoft.aad.reporting-appliedconditionalaccesspolicy.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|authenticationDetails|[authenticationDetail](../resources/microsoft.aad.reporting-authenticationdetail.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|authenticationMethodsUsed|String collection|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|authenticationProcessingDetails|[keyValue](../resources/microsoft.aad.reporting-keyvalue.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/microsoft.aad.reporting-authenticationrequirementpolicy.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|clientAppUsed|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|conditionalAccessStatus|conditionalAccessStatus|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|deviceDetail|[deviceDetail](../resources/microsoft.aad.reporting-devicedetail.md)|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|id|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|ipAddress|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|isInteractive|Boolean|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|location|[signInLocation](../resources/microsoft.aad.reporting-signinlocation.md)|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|mfaDetail|[mfaDetail](../resources/microsoft.aad.reporting-mfadetail.md)|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|networkLocationDetails|[networkLocationDetail](../resources/microsoft.aad.reporting-networklocationdetail.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|originalRequestId|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|processingTimeInMilliseconds|Int32|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|resourceDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|resourceId|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|riskDetail|riskDetail|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|riskEventType collection|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|riskLevelAggregated|riskLevel|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|riskLevel|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|servicePrincipalId|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|servicePrincipalName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|status|[signInStatus](../resources/microsoft.aad.reporting-signinstatus.md)|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|targetTenantId|Guid|**TODO: Add Description**|
|tokenIssuerName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|tokenIssuerType|tokenIssuerType|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userId|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userPrincipalName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|

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

