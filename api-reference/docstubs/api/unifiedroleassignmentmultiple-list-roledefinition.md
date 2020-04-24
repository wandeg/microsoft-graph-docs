---
title: "List roleDefinition"
description: "Get the unifiedRoleDefinitions from the roleDefinition navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List roleDefinition

Namespace: microsoft.graph

Get the unifiedRoleDefinitions from the roleDefinition navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/deviceManagement/roleAssignments/{unifiedRoleAssignmentMultipleId}/roleDefinition
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_unifiedroledefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/{unifiedRoleAssignmentMultipleId}/roleDefinition
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.unifiedroledefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
      "id": "58c5d3cf-d3cf-58c5-cfd3-c558cfd3c558",
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
  ]
}
```

