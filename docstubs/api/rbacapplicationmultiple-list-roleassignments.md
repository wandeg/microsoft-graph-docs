---
title: "List roleAssignments"
description: "Get the unifiedRoleAssignmentMultiples from the roleAssignments navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List roleAssignments

Namespace: microsoft.graph

Get the unifiedRoleAssignmentMultiples from the roleAssignments navigation property.

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
GET /roleManagement/deviceManagement/roleAssignments
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
If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.unifiedroleassignmentmultiple)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 550

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
      "id": "c1f044de-44de-c1f0-de44-f0c1de44f0c1",
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
  ]
}
```

