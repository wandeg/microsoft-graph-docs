---
title: "List mobileAppIntentAndStates"
description: "List properties and relationships of the mobileAppIntentAndState objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List mobileAppIntentAndStates

Namespace: microsoft.graph

List properties and relationships of the [mobileAppIntentAndState](../resources/mobileappintentandstate.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/mobileAppIntentAndStates
GET /users/{usersId}/mobileAppIntentAndStates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [mobileAppIntentAndState](../resources/mobileappintentandstate.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mobileappintentandstate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/mobileAppIntentAndStates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mobileappintentandstate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 992

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
      "id": "0e508b02-8b02-0e50-028b-500e028b500e",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "userId": "User Id value",
      "mobileAppList": [
        {
          "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
          "applicationId": "Application Id value",
          "displayName": "Display Name value",
          "mobileAppIntent": "String",
          "displayVersion": "Display Version value",
          "installState": "String",
          "supportedDeviceTypes": [
            {
              "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
              "type": "String",
              "minimumOperatingSystemVersion": "Minimum Operating System Version value",
              "maximumOperatingSystemVersion": "Maximum Operating System Version value"
            }
          ]
        }
      ]
    }
  ]
}
```

