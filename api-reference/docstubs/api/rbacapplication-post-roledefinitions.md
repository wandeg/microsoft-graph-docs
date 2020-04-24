---
title: "Create roleDefinitions"
description: "Create a new roleDefinitions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create roleDefinitions

Namespace: microsoft.graph

Create a new roleDefinitions object.

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
POST /roleManagement/directory/roleDefinitions
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
If successful, this method returns a `201 Created` response code and an [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
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
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedroledefinition"
}
-->
``` http
HTTP/1.1 201 Created
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

