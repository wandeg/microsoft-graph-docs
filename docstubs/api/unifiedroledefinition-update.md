---
title: "Update unifiedRoleDefinition"
description: "Update the properties of a unifiedRoleDefinition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update unifiedRoleDefinition

Namespace: microsoft.graph

Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.

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
PATCH /roleManagement/directory/roleDefinitions/{unifiedRoleDefinitionId}
PATCH /roleManagement/deviceManagement/roleDefinitions/{unifiedRoleDefinitionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.

The following table shows the properties that are required when you create the [unifiedRoleDefinition](../resources/unifiedroledefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|description|String||
|displayName|String||
|isBuiltIn|Boolean||
|isEnabled|Boolean||
|resourceScopes|String collection||
|rolePermissions|[unifiedRolePermission](../resources/unifiedrolepermission.md) collection||
|templateId|String||
|version|String||



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
Content-type: application/json
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 683

{
  "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
  "id": "ff5813a3-13a3-ff58-a313-58ffa31358ff",
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

