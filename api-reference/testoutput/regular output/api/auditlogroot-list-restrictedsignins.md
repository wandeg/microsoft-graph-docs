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

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [restrictedSignIn](../resources/restrictedsignin.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_restrictedsignin"
}
-->
``` http
GET https://graph.microsoft.com/localtest/auditLogs/restrictedSignIns
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.restrictedsignin)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2416

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.restrictedSignIn",
      "id": "0b687367-7367-0b68-6773-680b6773680b",
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
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
      "targetTenantId": "711ab416-b416-711a-16b4-1a7116b41a71"
    }
  ]
}
```

