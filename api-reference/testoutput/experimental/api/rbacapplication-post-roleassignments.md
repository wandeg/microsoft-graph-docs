---
title: "Add roleAssignments"
description: "Add roleAssignments by posting to the roleAssignments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add roleAssignments

Add roleAssignments by posting to the roleAssignments collection.

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
POST /roleManagement/directory/roleAssignments/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the unifiedRoleAssignment object.

The following table shows the properties that are required when you create the unifiedRoleAssignment.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|principalId|String||
|resourceScope|String||
|roleDefinitionId|String||



## Response
If successful, this method returns a `201 Created` response code and a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/roleManagement/directory/roleAssignments
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
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedroleassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 247

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "id": "c5fe217e-217e-c5fe-7e21-fec57e21fec5",
  "principalId": "Principal Id value",
  "resourceScope": "Resource Scope value",
  "roleDefinitionId": "Role Definition Id value"
}
```

