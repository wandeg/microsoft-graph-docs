---
title: "Update conversations"
description: "Update the properties of a conversations object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update conversations

Namespace: microsoft.graph

Update the properties of a conversations object.

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
PATCH /groups/{groupsId}/conversations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [conversation](../resources/conversation.md) object.

The following table shows the properties that are required when you create the [conversation](../resources/conversation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|topic|String|**TODO: Add Description**|
|hasAttachments|Boolean|**TODO: Add Description**|
|lastDeliveredDateTime|DateTimeOffset|**TODO: Add Description**|
|uniqueSenders|String collection|**TODO: Add Description**|
|preview|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [conversation](../resources/conversation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_conversations"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}/conversations
Content-Type: application/json
Content-length: 260

{
  "@odata.type": "#microsoft.graph.conversation",
  "topic": "Topic value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-12-31T23:58:05.2691795+03:00",
  "uniqueSenders": [
    "Unique Senders value"
  ],
  "preview": "Preview value"
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
  "@odata.type": "#microsoft.graph.conversation",
  "id": "b442aad6-aad6-b442-d6aa-42b4d6aa42b4",
  "topic": "Topic value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-12-31T23:58:05.2691795+03:00",
  "uniqueSenders": [
    "Unique Senders value"
  ],
  "preview": "Preview value"
}
```

