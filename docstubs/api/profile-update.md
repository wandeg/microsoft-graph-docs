---
title: "Update profile"
description: "Update the properties of a profile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update profile

Namespace: microsoft.graph

Update the properties of a [profile](../resources/profile.md) object.

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
PATCH /me/profile
PATCH /users/{usersId}/profile
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [profile](../resources/profile.md) object.

The following table shows the properties that are required when you create the [profile](../resources/profile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [profile](../resources/profile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_profile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile
Content-type: application/json
Content-length: 49

{
  "@odata.type": "#microsoft.graph.profile"
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
Content-Length: 98

{
  "@odata.type": "#microsoft.graph.profile",
  "id": "ee1ba496-a496-ee1b-96a4-1bee96a41bee"
}
```

