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

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/directory/roleDefinitions/{unifiedRoleDefinitionId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

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

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/roleManagement/directory/roleDefinitions/{unifiedRoleDefinitionId}
Content-type: application/json
Content-length: 545

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
      "condition": "Condition value"
    }
  ],
  "templateId": "Template Id value",
  "version": "Version value"
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
Content-Length: 594

{
  "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
  "id": "817a827d-827d-817a-7d82-7a817d827a81",
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
      "condition": "Condition value"
    }
  ],
  "templateId": "Template Id value",
  "version": "Version value"
}
```

