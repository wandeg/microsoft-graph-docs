---
title: "Update mention"
description: "Update the properties of a mention object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update mention

Update the properties of a [mention](../resources/mention.md) object.

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
PATCH /me/messages/{messageId}/mentions/{mentionId}
PATCH /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/mentions/{mentionId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [mention](../resources/mention.md) object.

The following table shows the properties that are required when you create the [mention](../resources/mention.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|mentioned|[emailAddress](../resources/emailAddress.md)||
|mentionText|String||
|clientReference|String||
|createdBy|[emailAddress](../resources/emailAddress.md)||
|createdDateTime|DateTimeOffset||
|serverCreatedDateTime|DateTimeOffset||
|deepLink|String||
|application|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [mention](../resources/mention.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_mention"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/me/messages/{messageId}/mentions/{mentionId}
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
  "serverCreatedDateTime": "2017-01-01T00:00:31.9976754+03:00",
  "deepLink": "Deep Link value",
  "application": "Application value"
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
Content-Length: 593

{
  "@odata.type": "#microsoft.graph.mention",
  "id": "8065beda-beda-8065-dabe-6580dabe6580",
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
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "serverCreatedDateTime": "2017-01-01T00:00:31.9976754+03:00",
  "deepLink": "Deep Link value",
  "application": "Application value"
}
```

