---
title: "Update privilegedRoleAssignment"
description: "Update the properties of a privilegedRoleAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update privilegedRoleAssignment

Namespace: microsoft.graph

Update the properties of a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.

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
PATCH /privilegedRoleAssignments/{privilegedRoleAssignmentsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.

The following table shows the properties that are required when you create the [privilegedRoleAssignment](../resources/privilegedroleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userId|String||
|roleId|String||
|isElevated|Boolean||
|expirationDateTime|DateTimeOffset||
|resultMessage|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_privilegedroleassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedRoleAssignments/{privilegedRoleAssignmentsId}
Content-type: application/json
Content-length: 255

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "isElevated": true,
  "expirationDateTime": "2017-01-01T00:00:46.7802483+03:00",
  "resultMessage": "Result Message value"
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
Content-Length: 304

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
  "id": "8a453401-3401-8a45-0134-458a0134458a",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "isElevated": true,
  "expirationDateTime": "2017-01-01T00:00:46.7802483+03:00",
  "resultMessage": "Result Message value"
}
```

