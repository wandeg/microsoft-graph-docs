---
title: "Update photos"
description: "Update the properties of a photos object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update photos

Namespace: microsoft.graph

Update the properties of a photos object.

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
PATCH /me/photos
PATCH /users/{usersId}/photos
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [profilePhoto](../resources/profilephoto.md) object.

The following table shows the properties that are required when you create the [profilePhoto](../resources/profilephoto.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|height|Int32|**TODO: Add Description**|
|width|Int32|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [profilePhoto](../resources/profilephoto.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_photos"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/photos
Content-Type: application/json
Content-length: 85

{
  "@odata.type": "#microsoft.graph.profilePhoto",
  "height": 6,
  "width": 5
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.profilePhoto",
  "id": "861907cf-07cf-8619-cf07-1986cf071986",
  "height": 6,
  "width": 5
}
```

