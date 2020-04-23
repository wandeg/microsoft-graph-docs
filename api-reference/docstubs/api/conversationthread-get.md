---
title: "Get conversationThread"
description: "Read the properties and relationships of a conversationThread object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get conversationThread

Namespace: microsoft.graph

Read the properties and relationships of a [conversationThread](../resources/conversationthread.md) object.

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
GET /groups/{groupsId}/threads/{conversationThreadId}
GET /invitations/{invitationsId}/invitedUser/joinedTeams/{groupId}/threads/{conversationThreadId}
GET /invitations/{invitationsId}/invitedUser/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}
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
If successful, this method returns a `200 OK` response code and a [conversationThread](../resources/conversationthread.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}
-->
``` http
GET https://graph.microsoft.com/beta/groups/{groupsId}/threads/{conversationThreadId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.conversationThread",
    "id": "a2eafdf3-fdf3-a2ea-f3fd-eaa2f3fdeaa2",
    "toRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient",
        "emailAddress": {
          "@odata.type": "microsoft.graph.emailAddress",
          "name": "Name value",
          "address": "Address value"
        }
      }
    ],
    "topic": "Topic value",
    "hasAttachments": true,
    "lastDeliveredDateTime": "2016-12-31T23:59:43.718822+03:00",
    "uniqueSenders": [
      "Unique Senders value"
    ],
    "ccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient"
      }
    ],
    "preview": "Preview value",
    "isLocked": true
  }
}
```

