---
title: "List hostedContents"
description: "Get the chatMessageHostedContents from the hostedContents navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List hostedContents

Namespace: microsoft.graph

Get the chatMessageHostedContents from the hostedContents navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/joinedGroups/{groupId}/team/channels/{channelId}/messages/{chatMessageId}/hostedContents
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/channels/{channelId}/messages/{chatMessageId}/hostedContents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.chatmessagehostedcontent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 156

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.chatMessageHostedContent",
      "id": "278a83bf-83bf-278a-bf83-8a27bf838a27"
    }
  ]
}
```

