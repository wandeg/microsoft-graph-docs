---
title: "Get mention"
description: "Read the properties and relationships of a mention object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get mention

Namespace: microsoft.graph

Read the properties and relationships of a [mention](../resources/mention.md) object.

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
GET /me/messages/{messageId}/mentions/{mentionId}
GET /users/{usersId}/messages/{messageId}/mentions/{mentionId}
GET /groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/mentions/{mentionId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [mention](../resources/mention.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_mention"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/messages/{messageId}/mentions/{mentionId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mention"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.mention",
    "id": "29373160-3160-2937-6031-372960313729",
    "mentioned": {
      "@odata.type": "microsoft.graph.emailAddress"
    },
    "mentionText": "String",
    "clientReference": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.emailAddress"
    },
    "createdDateTime": "String (timestamp)",
    "serverCreatedDateTime": "String (timestamp)",
    "deepLink": "String",
    "application": "String"
  }
}
```

