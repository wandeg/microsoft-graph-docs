---
title: "Update unifiedRoleDefinition"
description: "Update the properties of an unifiedRoleDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update unifiedRoleDefinition

Namespace: microsoft.graph

Update the properties of an [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.

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
PATCH /roleManagement/directory/roleDefinitions/{unifiedRoleDefinitionId}
PATCH /roleManagement/deviceManagement/roleDefinitions/{unifiedRoleDefinitionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.

The following table shows the properties that are required when you create the [unifiedRoleDefinition](../resources/unifiedroledefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|isBuiltIn|Boolean|**TODO: Add Description**|
|isEnabled|Boolean|**TODO: Add Description**|
|resourceScopes|String collection|**TODO: Add Description**|
|rolePermissions|[unifiedRolePermission](../resources/unifiedrolepermission.md) collection|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|
|version|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/{unifiedRoleDefinitionId}
Content-Type: application/json
Content-length: 634

{
  "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

