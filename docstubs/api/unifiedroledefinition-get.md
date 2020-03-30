---
title: "Get unifiedRoleDefinition"
description: "Read properties and relationships of the unifiedRoleDefinition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get unifiedRoleDefinition

Namespace: microsoft.graph

Read properties and relationships of the [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.

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
GET /roleManagement/directory/roleDefinitions/{unifiedRoleDefinitionId}
GET /roleManagement/deviceManagement/roleDefinitions/{unifiedRoleDefinitionId}
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
If successful, this method returns a `200 OK` response code and [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_unifiedroledefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/{unifiedRoleDefinitionId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 748

{
  "value": {
    "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
    "id": "02987cba-7cba-0298-ba7c-9802ba7c9802",
    "description": "Description value",
    "displayName": "Display Name value",
    "isBuiltIn": true,
    "isEnabled": true,
    "resourceScopes": [
      "Resource Scopes value"
    ],
    "rolePermissions": [
      {
        "@odata.type": "microsoft.graph.unifiedRolePermission",
        "allowedResourceActions": [
          "Allowed Resource Actions value"
        ],
        "excludedResourceActions": [
          "Excluded Resource Actions value"
        ],
        "condition": "Condition value"
      }
    ],
    "templateId": "Template Id value",
    "version": "Version value"
  }
}
```

