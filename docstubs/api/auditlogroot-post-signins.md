---
title: "Add signIns"
description: "Add signIns by posting to the signIns collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add signIns

Namespace: microsoft.graph

Add signIns by posting to the signIns collection.

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
POST /auditLogs/signIns/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [signIn](../resources/signin.md) object.

The following table shows the properties that are required when you create the [signIn](../resources/signin.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|alternateSignInName|String||
|appDisplayName|String||
|appId|String||
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection||
|authenticationDetails|[authenticationDetail](../resources/authenticationdetail.md) collection||
|authenticationMethodsUsed|String collection||
|authenticationProcessingDetails|[keyValue](../resources/keyvalue.md) collection||
|authenticationRequirement|String||
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md) collection||
|clientAppUsed|String||
|conditionalAccessStatus|Enumeration| Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String||
|createdDateTime|DateTimeOffset||
|deviceDetail|[deviceDetail](../resources/devicedetail.md)||
|isInteractive|Boolean||
|ipAddress|String||
|location|[signInLocation](../resources/signinlocation.md)||
|mfaDetail|[mfaDetail](../resources/mfadetail.md)||
|networkLocationDetails|[networkLocationDetail](../resources/networklocationdetail.md) collection||
|originalRequestId|String||
|processingTimeInMilliseconds|Int32||
|riskDetail|Enumeration| Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection| Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|riskEventTypes_v2|String collection||
|riskLevelAggregated|Enumeration| Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration| Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|resourceDisplayName|String||
|resourceId|String||
|servicePrincipalId|String||
|servicePrincipalName|String||
|status|[signInStatus](../resources/signinstatus.md)||
|tokenIssuerName|String||
|tokenIssuerType|Enumeration| Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String||
|userDisplayName|String||
|userId|String||
|userPrincipalName|String||



## Response
If successful, this method returns a `201 Created` response code and a [signIn](../resources/signin.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_signin_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/auditLogs/signIns
Content-type: application/json
Content-length: 3915

{
  "@odata.type": "#microsoft.graph.signIn",
  "alternateSignInName": "Alternate Sign In Name value",
  "appDisplayName": "App Display Name value",
  "appId": "App Id value",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy",
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
      "@odata.type": "microsoft.graph.authenticationDetail",
      "authenticationStepDateTime": "2017-01-01T00:02:33.516423+03:00",
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
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "authenticationRequirement": "Authentication Requirement value",
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy",
      "requirementProvider": "String",
      "detail": "Detail value"
    }
  ],
  "clientAppUsed": "Client App Used value",
  "conditionalAccessStatus": "String",
  "correlationId": "Correlation Id value",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail",
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
    "@odata.type": "microsoft.graph.signInLocation",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "geoCoordinates": {
      "@odata.type": "microsoft.graph.geoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double"
    }
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail",
    "authMethod": "Auth Method value",
    "authDetail": "Auth Detail value"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail",
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
  "riskEventTypes_v2": [
    "Risk Event Types_v2 value"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "Resource Id value",
  "servicePrincipalId": "Service Principal Id value",
  "servicePrincipalName": "Service Principal Name value",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signin"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4022

{
  "@odata.type": "#microsoft.graph.signIn",
  "id": "90c87cae-7cae-90c8-ae7c-c890ae7cc890",
  "alternateSignInName": "Alternate Sign In Name value",
  "appDisplayName": "App Display Name value",
  "appId": "App Id value",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy",
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
      "@odata.type": "microsoft.graph.authenticationDetail",
      "authenticationStepDateTime": "2017-01-01T00:02:33.516423+03:00",
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
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "authenticationRequirement": "Authentication Requirement value",
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy",
      "requirementProvider": "String",
      "detail": "Detail value"
    }
  ],
  "clientAppUsed": "Client App Used value",
  "conditionalAccessStatus": "String",
  "correlationId": "Correlation Id value",
  "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail",
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
    "@odata.type": "microsoft.graph.signInLocation",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "geoCoordinates": {
      "@odata.type": "microsoft.graph.geoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double"
    }
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail",
    "authMethod": "Auth Method value",
    "authDetail": "Auth Detail value"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail",
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
  "riskEventTypes_v2": [
    "Risk Event Types_v2 value"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "Resource Display Name value",
  "resourceId": "Resource Id value",
  "servicePrincipalId": "Service Principal Id value",
  "servicePrincipalName": "Service Principal Name value",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus",
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

