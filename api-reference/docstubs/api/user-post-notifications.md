---
title: "Create notifications"
description: "Create a new notifications object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create notifications

Namespace: microsoft.graph

Create a new notifications object.

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
POST /me/notifications
POST /users/{usersId}/notifications
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [notification](../resources/notification.md) object.

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
If successful, this method returns a `201 Created` response code and a [notification](../resources/notification.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_notification_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/notifications
Content-Type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.notification",
  "targetHostName": "String",
  "expirationDateTime": "String (timestamp)",
  "payload": {
    "@odata.type": "microsoft.graph.payloadTypes"
  },
  "displayTimeToLive": "Integer",
  "priority": "String",
  "groupName": "String",
  "targetPolicy": {
    "@odata.type": "microsoft.graph.targetPolicyEndpoints"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notification"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.notification",
  "id": "0f3879da-79da-0f38-da79-380fda79380f",
  "targetHostName": "String",
  "expirationDateTime": "String (timestamp)",
  "payload": {
    "@odata.type": "microsoft.graph.payloadTypes"
  },
  "displayTimeToLive": "Integer",
  "priority": "String",
  "groupName": "String",
  "targetPolicy": {
    "@odata.type": "microsoft.graph.targetPolicyEndpoints"
  }
}
```

