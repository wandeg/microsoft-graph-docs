---
title: "Update restrictedSignIns"
description: "Update the properties of a restrictedSignIns object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update restrictedSignIns

Namespace: Microsoft.AAD.Reporting

Update the properties of a restrictedSignIns object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /auditLogs/restrictedSignIns
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) object.

The following table shows the properties that are required when you create the [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md).

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
|isInteractive|Boolean|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|ipAddress|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|location|[signInLocation](../resources/microsoft.aad.reporting-signinlocation.md)|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|mfaDetail|[mfaDetail](../resources/microsoft.aad.reporting-mfadetail.md)|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|networkLocationDetails|[networkLocationDetail](../resources/microsoft.aad.reporting-networklocationdetail.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|originalRequestId|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|processingTimeInMilliseconds|Int32|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|riskDetail|riskDetail|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|riskEventType collection|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|riskLevelAggregated|riskLevel|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|riskLevel|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|resourceDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|resourceId|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|servicePrincipalId|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|servicePrincipalName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|status|[signInStatus](../resources/microsoft.aad.reporting-signinstatus.md)|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|tokenIssuerName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|tokenIssuerType|tokenIssuerType|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userId|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userPrincipalName|String|**TODO: Add Description** Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|targetTenantId|Guid|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_restrictedsignins"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/auditLogs/restrictedSignIns
Content-Type: application/json
Content-length: 1928

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
  "deviceDetail": {
    "@odata.type": "Microsoft.AAD.Reporting.deviceDetail"
  },
  "isInteractive": "Boolean",
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
  "processingTimeInMilliseconds": "Integer",
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

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
  "id": "ea2f1f97-1f97-ea2f-971f-2fea971f2fea",
  "isInteractive": "Boolean",
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
  "processingTimeInMilliseconds": "Integer",
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

