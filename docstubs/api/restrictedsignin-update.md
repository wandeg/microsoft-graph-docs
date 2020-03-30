---
title: "Update restrictedSignIn"
description: "Update the properties of a restrictedSignIn object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update restrictedSignIn

Namespace: microsoft.graph

Update the properties of a [restrictedSignIn](../resources/restrictedsignin.md) object.

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
PATCH /auditLogs/restrictedSignIns/{restrictedSignInId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [restrictedSignIn](../resources/restrictedsignin.md) object.

The following table shows the properties that are required when you create the [restrictedSignIn](../resources/restrictedsignin.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|alternateSignInName|String| Inherited from [signIn](../resources/signin.md)|
|appDisplayName|String| Inherited from [signIn](../resources/signin.md)|
|appId|String| Inherited from [signIn](../resources/signin.md)|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection| Inherited from [signIn](../resources/signin.md)|
|authenticationDetails|[authenticationDetail](../resources/authenticationdetail.md) collection| Inherited from [signIn](../resources/signin.md)|
|authenticationMethodsUsed|String collection| Inherited from [signIn](../resources/signin.md)|
|authenticationProcessingDetails|[keyValue](../resources/keyvalue.md) collection| Inherited from [signIn](../resources/signin.md)|
|authenticationRequirement|String| Inherited from [signIn](../resources/signin.md)|
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md) collection| Inherited from [signIn](../resources/signin.md)|
|clientAppUsed|String| Inherited from [signIn](../resources/signin.md)|
|conditionalAccessStatus|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String| Inherited from [signIn](../resources/signin.md)|
|createdDateTime|DateTimeOffset| Inherited from [signIn](../resources/signin.md)|
|deviceDetail|[deviceDetail](../resources/devicedetail.md)| Inherited from [signIn](../resources/signin.md)|
|isInteractive|Boolean| Inherited from [signIn](../resources/signin.md)|
|ipAddress|String| Inherited from [signIn](../resources/signin.md)|
|location|[signInLocation](../resources/signinlocation.md)| Inherited from [signIn](../resources/signin.md)|
|mfaDetail|[mfaDetail](../resources/mfadetail.md)| Inherited from [signIn](../resources/signin.md)|
|networkLocationDetails|[networkLocationDetail](../resources/networklocationdetail.md) collection| Inherited from [signIn](../resources/signin.md)|
|originalRequestId|String| Inherited from [signIn](../resources/signin.md)|
|processingTimeInMilliseconds|Int32| Inherited from [signIn](../resources/signin.md)|
|riskDetail|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|Enumeration collection| Inherited from [signIn](../resources/signin.md). Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|riskEventTypes_v2|String collection| Inherited from [signIn](../resources/signin.md)|
|riskLevelAggregated|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|resourceDisplayName|String| Inherited from [signIn](../resources/signin.md)|
|resourceId|String| Inherited from [signIn](../resources/signin.md)|
|servicePrincipalId|String| Inherited from [signIn](../resources/signin.md)|
|servicePrincipalName|String| Inherited from [signIn](../resources/signin.md)|
|status|[signInStatus](../resources/signinstatus.md)| Inherited from [signIn](../resources/signin.md)|
|tokenIssuerName|String| Inherited from [signIn](../resources/signin.md)|
|tokenIssuerType|Enumeration| Inherited from [signIn](../resources/signin.md). Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String| Inherited from [signIn](../resources/signin.md)|
|userDisplayName|String| Inherited from [signIn](../resources/signin.md)|
|userId|String| Inherited from [signIn](../resources/signin.md)|
|userPrincipalName|String| Inherited from [signIn](../resources/signin.md)|
|targetTenantId|Guid||



## Response
If successful, this method returns a `200 OK` response code and an updated [restrictedSignIn](../resources/restrictedsignin.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_restrictedsignin"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/auditLogs/restrictedSignIns/{restrictedSignInId}
Content-type: application/json
Content-length: 3987

{
  "@odata.type": "#microsoft.graph.restrictedSignIn",
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
      "authenticationStepDateTime": "2017-01-01T00:01:46.3230789+03:00",
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
  "userPrincipalName": "User Principal Name value",
  "targetTenantId": "877ecd01-cd01-877e-01cd-7e8701cd7e87"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4095

{
  "@odata.type": "#microsoft.graph.restrictedSignIn",
  "id": "abe2b8af-b8af-abe2-afb8-e2abafb8e2ab",
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
      "authenticationStepDateTime": "2017-01-01T00:01:46.3230789+03:00",
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
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
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
  "userPrincipalName": "User Principal Name value",
  "targetTenantId": "877ecd01-cd01-877e-01cd-7e8701cd7e87"
}
```

