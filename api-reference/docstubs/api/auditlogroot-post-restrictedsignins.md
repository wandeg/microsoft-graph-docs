---
title: "Create restrictedSignIns"
description: "Create a new restrictedSignIns object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create restrictedSignIns

Namespace: microsoft.graph

Create a new restrictedSignIns object.

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
POST /auditLogs/restrictedSignIns
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [restrictedSignIn](../resources/restrictedsignin.md) object.

The following table shows the properties that are required when you create the [restrictedSignIn](../resources/restrictedsignin.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|alternateSignInName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|appDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|appId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|authenticationDetails|[authenticationDetail](../resources/authenticationdetail.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|authenticationMethodsUsed|String collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|authenticationProcessingDetails|[keyValue](../resources/keyvalue.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|authenticationRequirement|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|clientAppUsed|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|conditionalAccessStatus|conditionalAccessStatus|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|deviceDetail|[deviceDetail](../resources/devicedetail.md)|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|isInteractive|Boolean|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|ipAddress|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|location|[signInLocation](../resources/signinlocation.md)|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|mfaDetail|[mfaDetail](../resources/mfadetail.md)|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|networkLocationDetails|[networkLocationDetail](../resources/networklocationdetail.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|originalRequestId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|processingTimeInMilliseconds|Int32|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|riskDetail|riskDetail|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|riskEventType collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|riskEventTypes_v2|String collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|riskLevelAggregated|riskLevel|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|riskLevel|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|resourceDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|resourceId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|servicePrincipalId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|servicePrincipalName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|status|[signInStatus](../resources/signinstatus.md)|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|tokenIssuerName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|tokenIssuerType|tokenIssuerType|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|userDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|userId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|userPrincipalName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|targetTenantId|Guid|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [restrictedSignIn](../resources/restrictedsignin.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_restrictedsignin_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/auditLogs/restrictedSignIns
Content-Type: application/json
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
      "authenticationStepDateTime": "2017-01-01T00:00:40.3373932+03:00",
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
  "targetTenantId": "0d778c92-8c92-0d77-928c-770d928c770d"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.restrictedsignin"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.restrictedSignIn",
  "id": "c182a2a2-a2a2-c182-a2a2-82c1a2a282c1",
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
      "authenticationStepDateTime": "2017-01-01T00:00:40.3373932+03:00",
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
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
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
  "targetTenantId": "0d778c92-8c92-0d77-928c-770d928c770d"
}
```

