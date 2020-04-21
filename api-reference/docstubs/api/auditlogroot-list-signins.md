---
title: "List signIns"
description: "Get the signIns from the signIns navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List signIns

Namespace: microsoft.graph

Get the signIns from the signIns navigation property.

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
GET /auditLogs/signIns
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
If successful, this method returns a `200 OK` response code and a collection of [signIn](../resources/signin.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_signin"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.signin)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.signIn",
      "id": "59b2917f-917f-59b2-7f91-b2597f91b259",
      "createdDateTime": "2017-01-01T00:01:28.5453509+00:00",
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
      "resourceId": "Resource Id value"
    }
  ]
}
```

