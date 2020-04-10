---
title: "List restrictedSignIns"
description: "Get the restrictedSignIns from the restrictedSignIns navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List restrictedSignIns

Namespace: microsoft.graph

Get the restrictedSignIns from the restrictedSignIns navigation property.

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
GET /auditLogs/restrictedSignIns
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
If successful, this method returns a `200 OK` response code and a collection of [restrictedSignIn](../resources/restrictedsignin.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_restrictedsignin"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/restrictedSignIns
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.restrictedsignin)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4612

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.restrictedSignIn",
      "id": "904cd10c-d10c-904c-0cd1-4c900cd14c90",
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
          "authenticationStepDateTime": "2016-12-31T23:58:51.3645044+00:00",
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
      "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
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
      "targetTenantId": "b9741705-1705-b974-0517-74b9051774b9"
    }
  ]
}
```

