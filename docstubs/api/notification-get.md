---
title: "Get notification"
description: "Read properties and relationships of the notification object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get notification

Namespace: microsoft.graph

Read properties and relationships of the [notification](../resources/notification.md) object.

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
GET /me/notifications/{notificationId}
GET /users/{usersId}/notifications/{notificationId}
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
If successful, this method returns a `200 OK` response code and [notification](../resources/notification.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_notification"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/notifications/{notificationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notification"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 774

{
  "value": {
    "@odata.type": "#microsoft.graph.notification",
    "id": "7b0b4154-4154-7b0b-5441-0b7b54410b7b",
    "targetHostName": "Target Host Name value",
    "expirationDateTime": "2016-12-31T23:58:22.4982594+03:00",
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
}
```

