---
title: "Get channel"
description: "Read properties and relationships of a channel object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get channel

Namespace: microsoft.graph

Read properties and relationships of a [channel](../resources/channel.md) object.

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
GET /teams/{teamsId}/primaryChannel
GET /teams/{teamsId}/channels/{channelId}
GET /me/joinedGroups/{groupId}/team/primaryChannel
GET /me/joinedGroups/{groupId}/team/channels/{channelId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_channel"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/primaryChannel
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.channel",
    "id": "0b8d74e8-74e8-0b8d-e874-8d0be8748d0b",
    "displayName": "Display Name value",
    "description": "Description value",
    "isFavoriteByDefault": true,
    "email": "Email value",
    "webUrl": "https://example.com/webUrl/",
    "membershipType": "String"
  }
}
```

