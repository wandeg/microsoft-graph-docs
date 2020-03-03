---
title: "Add notifications"
description: "Add notifications by posting to the notifications collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add notifications

Namespace: microsoft.graph

Add notifications by posting to the notifications collection.

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
POST /me/notifications/$ref
POST /users/{usersId}/notifications/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
|priority|Enumeration|. Possible values are: `None`, `High`, `Low`.|
|groupName|String||
|targetPolicy|[targetPolicyEndpoints](../resources/targetpolicyendpoints.md)||



## Response
If successful, this method returns a `201 Created` response code and a [notification](../resources/notification.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_notification_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/notifications
Content-type: application/json
Content-length: 662

{
  "@odata.type": "#microsoft.graph.notification",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 711

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
```

