---
title: "Update notification"
description: "Update the properties of a notification object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update notification

Namespace: microsoft.graph

Update the properties of a [notification](../resources/notification.md) object.

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
PATCH /me/notifications/{notificationId}
PATCH /users/{usersId}/notifications/{notificationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [notification](../resources/notification.md) object.

The following table shows the properties that are required when you create the [notification](../resources/notification.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|targetHostName|String||
|expirationDateTime|DateTimeOffset||
|payload|[payloadTypes](../resources/payloadtypes.md)||
|displayTimeToLive|Int32||
|priority|Enumeration| Possible values are: `None`, `High`, `Low`.|
|groupName|String||
|targetPolicy|[targetPolicyEndpoints](../resources/targetpolicyendpoints.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [notification](../resources/notification.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_notification"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/notifications/{notificationId}
Content-type: application/json
Content-length: 662

{
  "@odata.type": "#microsoft.graph.notification",
  "targetHostName": "Target Host Name value",
  "expirationDateTime": "2016-12-31T23:58:53.1230242+00:00",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 711

{
  "@odata.type": "#microsoft.graph.notification",
  "id": "ee028d2e-8d2e-ee02-2e8d-02ee2e8d02ee",
  "targetHostName": "Target Host Name value",
  "expirationDateTime": "2016-12-31T23:58:53.1230242+00:00",
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
```

