---
title: "Create mentions"
description: "Create a new mentions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create mentions

Namespace: microsoft.graph

Create a new mentions object.

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
POST /groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/mentions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [mention](../resources/mention.md) object.

The following table shows the properties that are required when you create the [mention](../resources/mention.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|mentioned|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description**|
|mentionText|String|**TODO: Add Description**|
|clientReference|String|**TODO: Add Description**|
|createdBy|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|serverCreatedDateTime|DateTimeOffset|**TODO: Add Description**|
|deepLink|String|**TODO: Add Description**|
|application|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [mention](../resources/mention.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_mention_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/mentions
Content-Type: application/json
Content-length: 362

{
  "@odata.type": "#microsoft.graph.mention",
  "mentioned": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "mentionText": "String",
  "clientReference": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "serverCreatedDateTime": "String (timestamp)",
  "deepLink": "String",
  "application": "String"
}
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
HTTP/1.1 201 Created
Content-Type: application/json
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
```

