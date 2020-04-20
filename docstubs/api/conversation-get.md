---
title: "Get conversation"
description: "Read properties and relationships of a conversation object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get conversation

Namespace: microsoft.graph

Read properties and relationships of a [conversation](../resources/conversation.md) object.

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
GET /groups/{groupsId}/conversations/{conversationId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/conversations/{conversationId}
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
If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}
-->
``` http
GET https://graph.microsoft.com/beta/groups/{groupsId}/conversations/{conversationId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.conversation",
    "id": "30565acb-5acb-3056-cb5a-5630cb5a5630",
    "topic": "Topic value",
    "hasAttachments": true,
    "lastDeliveredDateTime": "2016-12-31T23:57:30.9128732+03:00",
    "uniqueSenders": [
      "Unique Senders value"
    ],
    "preview": "Preview value"
  }
}
```

