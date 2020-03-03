---
title: "Create profilePhoto"
description: "Create a new profilePhoto object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create profilePhoto

Namespace: microsoft.graph

Create a new [profilePhoto](../resources/profilephoto.md) object.

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
POST /me/photos
POST /users/{usersId}/photos
POST /groups/{groupsId}/photos
POST /me/joinedTeams/{groupId}/photos
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [profilePhoto](../resources/profilephoto.md) object.

The following table shows the properties that are required when you create the [profilePhoto](../resources/profilephoto.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|height|Int32||
|width|Int32||



## Response
If successful, this method returns a `201 Created` response code and a [profilePhoto](../resources/profilephoto.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_profilephoto_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/photos
Content-type: application/json
Content-length: 85

{
  "@odata.type": "#microsoft.graph.profilePhoto",
  "height": 6,
  "width": 5
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilephoto"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 134

{
  "@odata.type": "#microsoft.graph.profilePhoto",
  "id": "ee96df92-df92-ee96-92df-96ee92df96ee",
  "height": 6,
  "width": 5
}
```

