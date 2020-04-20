---
title: "Update notifications"
description: "Update the properties of a notifications object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update notifications

Namespace: microsoft.graph

Update the properties of a notifications object.

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
PATCH /me/notifications
PATCH /users/{usersId}/notifications
PATCH /invitations/{invitationsId}/invitedUser/notifications
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [notification](../resources/notification.md) object.

The following table shows the properties that are required when you create the [notification](../resources/notification.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|targetHostName|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|payload|[payloadTypes](../resources/payloadtypes.md)|**TODO: Add Description**|
|displayTimeToLive|Int32|**TODO: Add Description**|
|priority|priority|**TODO: Add Description**. Possible values are: `None`, `High`, `Low`.|
|groupName|String|**TODO: Add Description**|
|targetPolicy|[targetPolicyEndpoints](../resources/targetpolicyendpoints.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [notification](../resources/notification.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_notifications"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/notifications
Content-Type: application/json
Content-length: 662

{
  "@odata.type": "#microsoft.graph.notification",
  "targetHostName": "Target Host Name value",
  "expirationDateTime": "2016-12-31T23:59:10.7331181+03:00",
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.notification",
  "id": "2c6f5bfc-5bfc-2c6f-fc5b-6f2cfc5b6f2c",
  "targetHostName": "Target Host Name value",
  "expirationDateTime": "2016-12-31T23:59:10.7331181+03:00",
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

