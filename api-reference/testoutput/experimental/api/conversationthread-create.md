---
title: "Create conversationThread"
description: "Create a new conversationThread object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create conversationThread

Namespace: microsoft.graph

Create a new [conversationThread](../resources/conversationthread.md) object.

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
POST /groups/{groupsId}/threads
POST /me/joinedGroups/{groupId}/threads
POST /me/joinedGroups/{groupId}/conversations/{conversationId}/threads
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [conversationThread](../resources/conversationthread.md) object.

The following table shows the properties that are required when you create the [conversationThread](../resources/conversationthread.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|toRecipients|[recipient](../resources/recipient.md) collection||
|topic|String||
|hasAttachments|Boolean||
|lastDeliveredDateTime|DateTimeOffset||
|uniqueSenders|String collection||
|ccRecipients|[recipient](../resources/recipient.md) collection||
|preview|String||
|isLocked|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [conversationThread](../resources/conversationthread.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/groups/{groupsId}/threads
Content-type: application/json
Content-length: 624

{
  "@odata.type": "#microsoft.graph.conversationThread",
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
  "lastDeliveredDateTime": "2016-12-31T23:58:15.3049+03:00",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationthread"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.conversationThread",
  "id": "3083ed6b-ed6b-3083-6bed-83306bed8330",
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
  "lastDeliveredDateTime": "2016-12-31T23:58:15.3049+03:00",
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
```

