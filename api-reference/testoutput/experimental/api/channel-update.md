---
title: "Update channel"
description: "Update the properties of a channel object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update channel

Update the properties of a [channel](../resources/channel.md) object.

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
PATCH /teams/{teamsId}/primaryChannel
PATCH /teams/{teamsId}/channels/{channelId}
PATCH /me/joinedGroups/{groupId}/team/primaryChannel
PATCH /me/joinedGroups/{groupId}/team/channels/{channelId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [channel](../resources/channel.md) object.

The following table shows the properties that are required when you create the [channel](../resources/channel.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|isFavoriteByDefault|Boolean||
|email|String||
|webUrl|String||
|membershipType|Enumeration|. Possible values are: `standard`, `private`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [channel](../resources/channel.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_channel"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/teams/{teamsId}/primaryChannel
Content-type: application/json
Content-length: 262

{
  "@odata.type": "#microsoft.graph.channel",
  "displayName": "Display Name value",
  "description": "Description value",
  "isFavoriteByDefault": true,
  "email": "Email value",
  "webUrl": "https://example.com/webUrl/",
  "membershipType": "String"
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
Content-Length: 311

{
  "@odata.type": "#microsoft.graph.channel",
  "id": "6eaa47f4-47f4-6eaa-f447-aa6ef447aa6e",
  "displayName": "Display Name value",
  "description": "Description value",
  "isFavoriteByDefault": true,
  "email": "Email value",
  "webUrl": "https://example.com/webUrl/",
  "membershipType": "String"
}
```

