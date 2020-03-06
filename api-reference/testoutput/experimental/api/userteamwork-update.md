---
title: "Update userTeamwork"
description: "Update the properties of a userTeamwork object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userTeamwork

Namespace: microsoft.graph

Update the properties of a [userTeamwork](../resources/userteamwork.md) object.

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
PATCH /me/teamwork
PATCH /users/{usersId}/teamwork
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userTeamwork](../resources/userteamwork.md) object.

The following table shows the properties that are required when you create the [userTeamwork](../resources/userteamwork.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [userTeamwork](../resources/userteamwork.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_userteamwork"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/me/teamwork
Content-type: application/json
Content-length: 54

{
  "@odata.type": "#microsoft.graph.userTeamwork"
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
Content-Length: 103

{
  "@odata.type": "#microsoft.graph.userTeamwork",
  "id": "63fc33a9-33a9-63fc-a933-fc63a933fc63"
}
```

