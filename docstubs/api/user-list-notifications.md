---
title: "List notifications"
description: "Get the notifications from the notifications navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List notifications

Namespace: microsoft.graph

Get the notifications from the notifications navigation property.

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
GET /users/{usersId}/notifications
GET /invitations/{invitationsId}/invitedUser/notifications
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
If successful, this method returns a `200 OK` response code and a collection of [notification](../resources/notification.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_notification"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/notifications
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.notification)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.notification",
      "id": "1fc1c2d3-c2d3-1fc1-d3c2-c11fd3c2c11f",
      "targetHostName": "Target Host Name value",
      "expirationDateTime": "2016-12-31T23:59:22.6673905+03:00",
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

