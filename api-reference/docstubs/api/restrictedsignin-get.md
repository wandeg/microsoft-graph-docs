---
title: "Get restrictedSignIn"
description: "Read the properties and relationships of a restrictedSignIn object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get restrictedSignIn

Namespace: microsoft.graph

Read the properties and relationships of a [restrictedSignIn](../resources/restrictedsignin.md) object.

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
GET /auditLogs/restrictedSignIns/{restrictedSignInId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [restrictedSignIn](../resources/restrictedsignin.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_restrictedsignin"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/restrictedSignIns/{restrictedSignInId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.restrictedSignIn"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.restrictedSignIn",
    "id": "26f03897-3897-26f0-9738-f0269738f026",
    "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
    "userDisplayName": "User Display Name value",
    "userPrincipalName": "User Principal Name value",
    "userId": "User Id value",
    "appId": "App Id value",
    "appDisplayName": "App Display Name value",
    "ipAddress": "Ip Address value",
    "status": {
      "@odata.type": "microsoft.graph.signInStatus",
      "errorCode": 9,
      "failureReason": "Failure Reason value",
      "additionalDetails": "Additional Details value"
    },
    "clientAppUsed": "Client App Used value",
    "deviceDetail": {
      "@odata.type": "microsoft.graph.deviceDetail",
      "deviceId": "Device Id value",
      "displayName": "Display Name value",
      "operatingSystem": "Operating System value",
      "browser": "Browser value",
      "isCompliant": true,
      "isManaged": true,
      "trustType": "Trust Type value"
    },
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
    "correlationId": "Correlation Id value",
    "conditionalAccessStatus": "String",
    "appliedConditionalAccessPolicies": [
      {
        "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy",
        "id": "Id value",
        "enforcedGrantControls": [
          "Enforced Grant Controls value"
        ],
        "enforcedSessionControls": [
          "Enforced Session Controls value"
        ],
        "result": "String"
      }
    ],
    "isInteractive": true,
    "riskDetail": "String",
    "riskLevelAggregated": "String",
    "riskLevelDuringSignIn": "String",
    "riskState": "String",
    "riskEventTypes": [
      "String"
    ],
    "resourceDisplayName": "Resource Display Name value",
    "resourceId": "Resource Id value",
    "targetTenantId": "492e3696-3696-492e-9636-2e4996362e49"
  }
}
```

