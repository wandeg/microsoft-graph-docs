---
title: "List mentions"
description: "Get the mentions from the mentions navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List mentions

Namespace: microsoft.graph

Get the mentions from the mentions navigation property.

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
GET /groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/mentions
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

If successful, this method returns a `200 OK` response code and a collection of [mention](../resources/mention.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_mention"
}
-->
``` http
GET https://graph.microsoft.com/beta/groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/mentions
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mention)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
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
  ]
}
```

