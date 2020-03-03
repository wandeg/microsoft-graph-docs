---
title: "Add mentions"
description: "Add mentions by posting to the mentions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add mentions

Namespace: microsoft.graph

Add mentions by posting to the mentions collection.

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
POST /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/mentions/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [mention](../resources/mention.md) object.

The following table shows the properties that are required when you create the [mention](../resources/mention.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|mentioned|[emailAddress](../resources/emailaddress.md)||
|mentionText|String||
|clientReference|String||
|createdBy|[emailAddress](../resources/emailaddress.md)||
|createdDateTime|DateTimeOffset||
|serverCreatedDateTime|DateTimeOffset||
|deepLink|String||
|application|String||



## Response
If successful, this method returns a `201 Created` response code and a [mention](../resources/mention.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mention_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/mentions
Content-type: application/json
Content-length: 485

{
  "@odata.type": "#microsoft.graph.mention",
  "mentioned": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "Name value",
    "address": "Address value"
  },
  "mentionText": "Mention Text value",
  "clientReference": "Client Reference value",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "serverCreatedDateTime": "2016-12-31T23:57:52.2165536+03:00",
  "deepLink": "Deep Link value",
  "application": "Application value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mention"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 592

{
  "@odata.type": "#microsoft.graph.mention",
  "id": "97080269-0269-9708-6902-089769020897",
  "mentioned": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "Name value",
    "address": "Address value"
  },
  "mentionText": "Mention Text value",
  "clientReference": "Client Reference value",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "serverCreatedDateTime": "2016-12-31T23:57:52.2165536+03:00",
  "deepLink": "Deep Link value",
  "application": "Application value"
}
```

