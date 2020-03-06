---
title: "Get unifiedRoleAssignment"
description: "Read properties and relationships of the unifiedRoleAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get unifiedRoleAssignment

Namespace: microsoft.graph

Read properties and relationships of the [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.

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
GET /roleManagement/directory/roleAssignments/{unifiedRoleAssignmentId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}
-->
``` http
GET https://graph.microsoft.com/localtest/roleManagement/directory/roleAssignments/{unifiedRoleAssignmentId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 276

{
  "value": {
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "id": "6a6b358e-358e-6a6b-8e35-6b6a8e356b6a",
    "principalId": "Principal Id value",
    "resourceScope": "Resource Scope value",
    "roleDefinitionId": "Role Definition Id value"
  }
}
```

