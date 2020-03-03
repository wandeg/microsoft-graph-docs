---
title: "Update unifiedRoleAssignment"
description: "Update the properties of a unifiedRoleAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update unifiedRoleAssignment

Namespace: microsoft.graph

Update the properties of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.

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
PATCH /roleManagement/directory/roleAssignments/{unifiedRoleAssignmentId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.

The following table shows the properties that are required when you create the [unifiedRoleAssignment](../resources/unifiedroleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|principalId|String||
|resourceScope|String||
|roleDefinitionId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/roleManagement/directory/roleAssignments/{unifiedRoleAssignmentId}
Content-type: application/json
Content-length: 198

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "principalId": "Principal Id value",
  "resourceScope": "Resource Scope value",
  "roleDefinitionId": "Role Definition Id value"
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
Content-Length: 247

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "id": "dfc82d60-2d60-dfc8-602d-c8df602dc8df",
  "principalId": "Principal Id value",
  "resourceScope": "Resource Scope value",
  "roleDefinitionId": "Role Definition Id value"
}
```

