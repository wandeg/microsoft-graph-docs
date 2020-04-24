---
title: "Update chatMessageHostedContent"
description: "Update the properties of a chatMessageHostedContent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update chatMessageHostedContent

Namespace: microsoft.graph

Update the properties of a [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.

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
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/channels/{channelId}/messages/{chatMessageId}/hostedContents/{chatMessageHostedContentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.

The following table shows the properties that are required when you create the [chatMessageHostedContent](../resources/chatmessagehostedcontent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_chatmessagehostedcontent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/channels/{channelId}/messages/{chatMessageId}/hostedContents/{chatMessageHostedContentId}
Content-Type: application/json
Content-length: 66

{
  "@odata.type": "#microsoft.graph.chatMessageHostedContent"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.chatMessageHostedContent",
  "id": "d9fdca2f-ca2f-d9fd-2fca-fdd92fcafdd9"
}
```

