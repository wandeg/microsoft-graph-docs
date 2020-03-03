---
title: "Create chatMessageHostedContent"
description: "Create a new chatMessageHostedContent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create chatMessageHostedContent

Namespace: microsoft.graph

Create a new [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.

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
POST /me/joinedGroups/{groupId}/team/channels/{channelId}/messages/{chatMessageId}/hostedContents
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.

The following table shows the properties that are required when you create the [chatMessageHostedContent](../resources/chatmessagehostedcontent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_chatmessagehostedcontent_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/team/channels/{channelId}/messages/{chatMessageId}/hostedContents
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
  "truncated": true,
  "@odata.type": "microsoft.graph.chatmessagehostedcontent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 115

{
  "@odata.type": "#microsoft.graph.chatMessageHostedContent",
  "id": "c92830a1-30a1-c928-a130-28c9a13028c9"
}
```

