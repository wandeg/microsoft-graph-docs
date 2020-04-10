---
title: "Get unifiedRoleAssignmentMultiple"
description: "Read properties and relationships of the unifiedRoleAssignmentMultiple object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get unifiedRoleAssignmentMultiple

Namespace: microsoft.graph

Read properties and relationships of the [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.

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
GET /roleManagement/deviceManagement/roleAssignments/{unifiedRoleAssignmentMultipleId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/{unifiedRoleAssignmentMultipleId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 506

{
  "value": {
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "9c6c6b16-6b16-9c6c-166b-6c9c166b6c9c",
    "roleDefinitionId": "Role Definition Id value",
    "condition": "Condition value",
    "displayName": "Display Name value",
    "description": "Description value",
    "principalIds": [
      "Principal Ids value"
    ],
    "directoryScopeIds": [
      "Directory Scope Ids value"
    ],
    "appScopeIds": [
      "App Scope Ids value"
    ]
  }
}
```

