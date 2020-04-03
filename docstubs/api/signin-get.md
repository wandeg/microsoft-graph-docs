---
title: "Get signIn"
description: "Read properties and relationships of the signIn object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get signIn

Namespace: microsoft.graph

Read properties and relationships of the [signIn](../resources/signin.md) object.

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
GET /auditLogs/signIns/{signInId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_signin"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{signInId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4283

{
  "value": {
    "@odata.type": "#microsoft.graph.signIn",
    "id": "0f77e869-e869-0f77-69e8-770f69e8770f",
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
        "authenticationStepDateTime": "2017-01-01T00:01:24.6504342+00:00",
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
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
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
}
```

