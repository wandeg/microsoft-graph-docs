---
title: "List notifications"
description: "Get the notifications from the notifications navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
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
GET /me/notifications
GET /users/{usersId}/notifications
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
GET https://graph.microsoft.com/beta/me/notifications
```

### Response
**Note:** The response object shown here might be shortened for readability.
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
      "id": "2eaa9529-9529-2eaa-2995-aa2e2995aa2e",
      "targetHostName": "Target Host Name value",
      "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
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

