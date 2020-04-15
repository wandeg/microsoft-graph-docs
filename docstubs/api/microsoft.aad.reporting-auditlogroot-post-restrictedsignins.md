---
title: "Add restrictedSignIns"
description: "Add restrictedSignIns by posting to the restrictedSignIns collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add restrictedSignIns

Namespace: Microsoft.AAD.Reporting

Add restrictedSignIns by posting to the restrictedSignIns collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /auditLogs/restrictedSignIns/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) object.

The following table shows the properties that are required when you create the [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md).

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
|isInteractive|Boolean| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|ipAddress|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|location|[signInLocation](../resources/microsoft.aad.reporting-signinlocation.md)| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|mfaDetail|[mfaDetail](../resources/microsoft.aad.reporting-mfadetail.md)| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|networkLocationDetails|[networkLocationDetail](../resources/microsoft.aad.reporting-networklocationdetail.md) collection| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|originalRequestId|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|processingTimeInMilliseconds|Int32| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|riskDetail|Enumeration| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|riskLevelAggregated|Enumeration| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|resourceDisplayName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|resourceId|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|servicePrincipalId|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|servicePrincipalName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|status|[signInStatus](../resources/microsoft.aad.reporting-signinstatus.md)| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|tokenIssuerName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|tokenIssuerType|Enumeration| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md). Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userDisplayName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userId|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|userPrincipalName|String| Inherited from [signIn](../resources/microsoft.aad.reporting-signin.md)|
|targetTenantId|Guid||



## Response
If successful, this method returns a `201 Created` response code and a [restrictedSignIn](../resources/microsoft.aad.reporting-restrictedsignin.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_restrictedsignin_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/auditLogs/restrictedSignIns
Content-type: application/json
Content-length: 3941

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
      "authenticationStepDateTime": "2017-01-01T00:02:11.988433+00:00",
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
  "targetTenantId": "4c1db47b-b47b-4c1d-7bb4-1d4c7bb41d4c"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.aad.reporting.restrictedsignin"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4049

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
      "authenticationStepDateTime": "2017-01-01T00:02:11.988433+00:00",
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
  "createdDateTime": "2017-01-01T00:03:26.3279546+00:00",
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
  "id": "10cfc312-c312-10cf-12c3-cf1012c3cf10",
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
  "targetTenantId": "4c1db47b-b47b-4c1d-7bb4-1d4c7bb41d4c"
}
```

