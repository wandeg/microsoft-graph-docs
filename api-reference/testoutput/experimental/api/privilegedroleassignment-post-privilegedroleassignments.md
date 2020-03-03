---
title: "Create privilegedRoleAssignment"
description: "Create a new privilegedRoleAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create privilegedRoleAssignment

Namespace: microsoft.graph

Create a new [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.

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
POST /privilegedRoleAssignments
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}
-->
``` http
POST https://graph.microsoft.com/localtest/privilegedRoleAssignments
Content-type: application/json
Content-length: 255

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "isElevated": true,
  "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
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
  "id": "59a88cae-8cae-59a8-ae8c-a859ae8ca859",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "isElevated": true,
  "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
  "resultMessage": "Result Message value"
}
```

