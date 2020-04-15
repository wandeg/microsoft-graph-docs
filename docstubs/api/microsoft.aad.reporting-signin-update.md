---
title: "Update signIn"
description: "Update the properties of a signIn object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update signIn

Namespace: Microsoft.AAD.Reporting

Update the properties of a [signIn](../resources/microsoft.aad.reporting-signin.md) object.

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
PATCH /auditLogs/signIns/{signInId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [signIn](../resources/microsoft.aad.reporting-signin.md) object.

The following table shows the properties that are required when you create the [signIn](../resources/microsoft.aad.reporting-signin.md).

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
|isInteractive|Boolean||
|ipAddress|String||
|location|[signInLocation](../resources/microsoft.aad.reporting-signinlocation.md)||
|mfaDetail|[mfaDetail](../resources/microsoft.aad.reporting-mfadetail.md)||
|networkLocationDetails|[networkLocationDetail](../resources/microsoft.aad.reporting-networklocationdetail.md) collection||
|originalRequestId|String||
|processingTimeInMilliseconds|Int32||
|riskDetail|Enumeration| Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection| Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|riskLevelAggregated|Enumeration| Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration| Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|resourceDisplayName|String||
|resourceId|String||
|servicePrincipalId|String||
|servicePrincipalName|String||
|status|[signInStatus](../resources/microsoft.aad.reporting-signinstatus.md)||
|tokenIssuerName|String||
|tokenIssuerType|Enumeration| Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String||
|userDisplayName|String||
|userId|String||
|userPrincipalName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [signIn](../resources/microsoft.aad.reporting-signin.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_signin"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/auditLogs/signIns/{signInId}
Content-type: application/json
Content-length: 3870

{
  "@odata.type": "#Microsoft.AAD.Reporting.signIn",
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
  "userPrincipalName": "User Principal Name value"
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
Content-Length: 3978

{
  "@odata.type": "#Microsoft.AAD.Reporting.signIn",
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
  "id": "84d44cf6-4cf6-84d4-f64c-d484f64cd484",
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
  "userPrincipalName": "User Principal Name value"
}
```

