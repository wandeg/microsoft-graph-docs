---
title: "conversationThread: reply"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# reply

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /groups/{groupsId}/threads/{conversationThreadId}/reply
POST /invitations/{invitationsId}/invitedUser/joinedTeams/{groupId}/threads/{conversationThreadId}/reply
POST /invitations/{invitationsId}/invitedUser/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/reply
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|Post|[post](../resources/post.md)|**TODO: Add Description**|



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/threads/{conversationThreadId}/reply

Content-Type: application/json
Content-length: 928

{
  "Post": {
    "@odata.type": "#microsoft.graph.post",
    "id": "296cccf5-ccf5-296c-f5cc-6c29f5cc6c29",
    "createdDateTime": "2017-01-01T00:01:28.5453509+00:00",
    "lastModifiedDateTime": "2017-01-01T00:01:26.0388723+00:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "body": {
      "@odata.type": "microsoft.graph.itemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "receivedDateTime": "2016-12-31T23:57:43.1694496+00:00",
    "hasAttachments": true,
    "from": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "sender": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "conversationThreadId": "Conversation Thread Id value",
    "newParticipants": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "conversationId": "Conversation Id value"
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
HTTP/1.1 204 No Content
```

