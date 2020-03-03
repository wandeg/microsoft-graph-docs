---
title: "List notifications"
description: "List properties and relationships of the notification objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List notifications

Namespace: microsoft.graph

List properties and relationships of the [notification](../resources/notification.md) objects.

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
GET /me/notifications
GET /users/{usersId}/notifications
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [notification](../resources/notification.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_notification"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/notifications
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.notification)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 832

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.notification",
      "id": "d3e59931-9931-d3e5-3199-e5d33199e5d3",
      "targetHostName": "Target Host Name value",
      "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
      "payload": {
        "@odata.type": "microsoft.graph.payloadTypes",
        "rawContent": "Raw Content value",
        "visualContent": {
          "@odata.type": "microsoft.graph.visualProperties",
          "title": "Title value",
          "body": "Body value"
        }
      },
      "displayTimeToLive": 1,
      "priority": "String",
      "groupName": "Group Name value",
      "targetPolicy": {
        "@odata.type": "microsoft.graph.targetPolicyEndpoints",
        "platformTypes": [
          "Platform Types value"
        ]
      }
    }
  ]
}
```

