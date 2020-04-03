---
title: "Create assignments"
description: "Create assignments by posting to the assignments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create assignments

Namespace: microsoft.graph

Create assignments by posting to the assignments collection.

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
POST /privilegedRoles/{privilegedRolesId}/assignments/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedRoles/{privilegedRolesId}/assignments
Content-type: application/json
Content-length: 255

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "isElevated": true,
  "expirationDateTime": "2016-12-31T23:57:47.0232285+00:00",
  "resultMessage": "Result Message value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedroleassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 304

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
  "id": "18ccd93a-d93a-18cc-3ad9-cc183ad9cc18",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "isElevated": true,
  "expirationDateTime": "2016-12-31T23:57:47.0232285+00:00",
  "resultMessage": "Result Message value"
}
```

