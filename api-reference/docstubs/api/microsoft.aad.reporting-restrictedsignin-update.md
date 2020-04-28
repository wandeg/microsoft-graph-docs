---
title: "Update restrictedSignIn"
description: "Update the properties of a restrictedSignIn object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update restrictedSignIn

Namespace: Microsoft.AAD.Reporting

Update the properties of a [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) object.

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
PATCH /auditLogs/restrictedSignIns/{restrictedSignInId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) object.

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
  "name": "update_restrictedsignin"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/auditLogs/restrictedSignIns/{restrictedSignInId}
Content-Type: application/json
Content-length: 3942

{
  "@odata.type": "#Microsoft.AAD.Reporting.restrictedSignIn",
  "alternateSignInName": "Alternate Sign In Name value",
  "appDisplayName": "App Display Name value",
  "appId": "App Id value",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.appliedConditionalAccessPolicy",
      "id": "Id value",
      "displayName": "Display Name value",
      "enforcedGrantControls": [
        "Enforced Grant Controls value"
      ],
      "enforcedSessionControls": [
        "Enforced Session Controls value"
      ],
      "conditionsSatisfied": "String",
      "conditionsNotSatisfied": "String",
      "result": "String"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.authenticationDetail",
      "authenticationStepDateTime": "2016-12-31T23:59:41.5324069+00:00",
      "authenticationMethod": "Authentication Method value",
      "authenticationMethodDetail": "Authentication Method Detail value",
      "succeeded": true,
      "authenticationStepResultDetail": "Authentication Step Result Detail value",
      "authenticationStepRequirement": "Authentication Step Requirement value"
    }
  ],
  "authenticationMethodsUsed": [
    "Authentication Methods Used value"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.authenticationRequirementPolicy",
      "requirementProvider": "String",
      "detail": "Detail value"
    }
  ],
  "clientAppUsed": "Client App Used value",
  "conditionalAccessStatus": "String",
  "correlationId": "Correlation Id value",
  "deviceDetail": {
    "@odata.type": "Microsoft.AAD.Reporting.deviceDetail",
    "deviceId": "Device Id value",
    "operatingSystem": "Operating System value",
    "browser": "Browser value",
    "browserId": "Browser Id value",
    "isCompliant": true,
    "isManaged": true,
    "trustType": "Trust Type value"
  },
  "isInteractive": true,
  "ipAddress": "Ip Address value",
  "location": {
    "@odata.type": "Microsoft.AAD.Reporting.signInLocation",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "geoCoordinates": {
      "@odata.type": "Microsoft.AAD.Reporting.geoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double"
    }
  },
  "mfaDetail": {
    "@odata.type": "Microsoft.AAD.Reporting.mfaDetail",
    "authMethod": "Auth Method value",
    "authDetail": "Auth Detail value"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.networkLocationDetail",
      "networkType": "String",
      "networkNames": [
        "Network Names value"
      ]
    }
  ],
  "originalRequestId": "Original Request Id value",
  "processingTimeInMilliseconds": 12,
  "riskDetail": "String",
  "riskEventTypes": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "Resource Id value",
  "servicePrincipalId": "Service Principal Id value",
  "servicePrincipalName": "Service Principal Name value",
  "status": {
    "@odata.type": "Microsoft.AAD.Reporting.signInStatus",
    "errorCode": 9,
    "failureReason": "Failure Reason value",
    "additionalDetails": "Additional Details value"
  },
  "tokenIssuerName": "Token Issuer Name value",
  "tokenIssuerType": "String",
  "userAgent": "User Agent value",
  "userDisplayName": "User Display Name value",
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value",
  "targetTenantId": "39314ba8-4ba8-3931-a84b-3139a84b3139"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
  "alternateSignInName": "Alternate Sign In Name value",
  "appDisplayName": "App Display Name value",
  "appId": "App Id value",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.appliedConditionalAccessPolicy",
      "id": "Id value",
      "displayName": "Display Name value",
      "enforcedGrantControls": [
        "Enforced Grant Controls value"
      ],
      "enforcedSessionControls": [
        "Enforced Session Controls value"
      ],
      "conditionsSatisfied": "String",
      "conditionsNotSatisfied": "String",
      "result": "String"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.authenticationDetail",
      "authenticationStepDateTime": "2016-12-31T23:59:41.5324069+00:00",
      "authenticationMethod": "Authentication Method value",
      "authenticationMethodDetail": "Authentication Method Detail value",
      "succeeded": true,
      "authenticationStepResultDetail": "Authentication Step Result Detail value",
      "authenticationStepRequirement": "Authentication Step Requirement value"
    }
  ],
  "authenticationMethodsUsed": [
    "Authentication Methods Used value"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.authenticationRequirementPolicy",
      "requirementProvider": "String",
      "detail": "Detail value"
    }
  ],
  "clientAppUsed": "Client App Used value",
  "conditionalAccessStatus": "String",
  "correlationId": "Correlation Id value",
  "createdDateTime": "2016-12-31T23:59:18.0340888+00:00",
  "deviceDetail": {
    "@odata.type": "Microsoft.AAD.Reporting.deviceDetail",
    "deviceId": "Device Id value",
    "operatingSystem": "Operating System value",
    "browser": "Browser value",
    "browserId": "Browser Id value",
    "isCompliant": true,
    "isManaged": true,
    "trustType": "Trust Type value"
  },
  "id": "47acee84-ee84-47ac-84ee-ac4784eeac47",
  "isInteractive": true,
  "ipAddress": "Ip Address value",
  "location": {
    "@odata.type": "Microsoft.AAD.Reporting.signInLocation",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "geoCoordinates": {
      "@odata.type": "Microsoft.AAD.Reporting.geoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double"
    }
  },
  "mfaDetail": {
    "@odata.type": "Microsoft.AAD.Reporting.mfaDetail",
    "authMethod": "Auth Method value",
    "authDetail": "Auth Detail value"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "Microsoft.AAD.Reporting.networkLocationDetail",
      "networkType": "String",
      "networkNames": [
        "Network Names value"
      ]
    }
  ],
  "originalRequestId": "Original Request Id value",
  "processingTimeInMilliseconds": 12,
  "riskDetail": "String",
  "riskEventTypes": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "Resource Id value",
  "servicePrincipalId": "Service Principal Id value",
  "servicePrincipalName": "Service Principal Name value",
  "status": {
    "@odata.type": "Microsoft.AAD.Reporting.signInStatus",
    "errorCode": 9,
    "failureReason": "Failure Reason value",
    "additionalDetails": "Additional Details value"
  },
  "tokenIssuerName": "Token Issuer Name value",
  "tokenIssuerType": "String",
  "userAgent": "User Agent value",
  "userDisplayName": "User Display Name value",
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value",
  "targetTenantId": "39314ba8-4ba8-3931-a84b-3139a84b3139"
}
```

