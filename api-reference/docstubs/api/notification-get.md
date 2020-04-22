---
title: "Get notification"
description: "Read properties and relationships of a notification object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get notification

Namespace: microsoft.graph

Read properties and relationships of a [notification](../resources/notification.md) object.

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
GET /me/notifications/{notificationId}
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
If successful, this method returns a `200 OK` response code and a [notification](../resources/notification.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_notification"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/notifications/{notificationId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notification"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.notification",
    "id": "d2817ac1-7ac1-d281-c17a-81d2c17a81d2",
    "targetHostName": "Target Host Name value",
    "expirationDateTime": "2016-12-31T23:57:47.1330234+00:00",
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

