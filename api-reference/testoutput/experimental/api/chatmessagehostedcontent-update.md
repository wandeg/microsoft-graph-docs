---
title: "Update chatMessageHostedContent"
description: "Update the properties of a chatMessageHostedContent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update chatMessageHostedContent

Namespace: microsoft.graph

Update the properties of a [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.

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
PATCH /me/joinedGroups/{groupId}/team/channels/{channelId}/messages/{chatMessageId}/hostedContents/{chatMessageHostedContentId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.

The following table shows the properties that are required when you create the [chatMessageHostedContent](../resources/chatmessagehostedcontent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_chatmessagehostedcontent"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/team/channels/{channelId}/messages/{chatMessageId}/hostedContents/{chatMessageHostedContentId}
Content-type: application/json
Content-length: 66

{
  "@odata.type": "#microsoft.graph.chatMessageHostedContent"
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
Content-Length: 115

{
  "@odata.type": "#microsoft.graph.chatMessageHostedContent",
  "id": "c92830a1-30a1-c928-a130-28c9a13028c9"
}
```

