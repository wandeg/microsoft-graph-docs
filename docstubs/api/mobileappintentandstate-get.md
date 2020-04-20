---
title: "Get mobileAppIntentAndState"
description: "Read properties and relationships of a mobileAppIntentAndState object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get mobileAppIntentAndState

Namespace: microsoft.graph

Read properties and relationships of a [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object.

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
GET /me/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
GET /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
GET /invitations/{invitationsId}/invitedUser/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
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
If successful, this method returns a `200 OK` response code and a [mobileAppIntentAndState](../resources/mobileappintentandstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_mobileappintentandstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileAppIntentAndState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
    "id": "8d47b4f3-b4f3-8d47-f3b4-478df3b4478d",
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
}
```

