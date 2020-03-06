---
title: "List signIns"
description: "Get the signIns from the signIns navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List signIns

Namespace: microsoft.graph

Get the signIns from the signIns navigation property.

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
GET /auditLogs/signIns
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [signIn](../resources/signin.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_signin"
}
-->
``` http
GET https://graph.microsoft.com/localtest/auditLogs/signIns
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.signin)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4388

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.signIn",
      "id": "15f5fb5d-fb5d-15f5-5dfb-f5155dfbf515",
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
          "authenticationStepDateTime": "2016-12-31T23:57:38.2707349+03:00",
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
      "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
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
  ]
}
```

