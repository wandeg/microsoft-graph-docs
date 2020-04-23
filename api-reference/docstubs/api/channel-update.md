---
title: "Update channel"
description: "Update the properties of a channel object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update channel

Namespace: microsoft.graph

Update the properties of a [channel](../resources/channel.md) object.

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
PATCH /teams/{teamsId}/channels/{channelId}
PATCH /invitations/{invitationsId}/invitedUser/joinedTeams/{groupId}/team/channels/{channelId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [channel](../resources/channel.md) object.

The following table shows the properties that are required when you create the [channel](../resources/channel.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [channel](../resources/channel.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_channel"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/{teamsId}/channels/{channelId}
Content-Type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.channel",
  "displayName": "Display Name value",
  "description": "Description value",
  "email": "Email value",
  "webUrl": "https://example.com/webUrl/"
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
  "@odata.type": "#microsoft.graph.channel",
  "id": "d4c81537-1537-d4c8-3715-c8d43715c8d4",
  "displayName": "Display Name value",
  "description": "Description value",
  "email": "Email value",
  "webUrl": "https://example.com/webUrl/"
}
```

