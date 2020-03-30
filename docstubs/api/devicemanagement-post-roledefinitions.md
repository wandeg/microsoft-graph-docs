---
title: "Add roleDefinitions"
description: "Add roleDefinitions by posting to the roleDefinitions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add roleDefinitions

Namespace: microsoft.graph

Add roleDefinitions by posting to the roleDefinitions collection.

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
POST /deviceManagement/roleDefinitions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [roleDefinition](../resources/roledefinition.md) object.

The following table shows the properties that are required when you create the [roleDefinition](../resources/roledefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|permissions|[rolePermission](../resources/rolepermission.md) collection||
|rolePermissions|[rolePermission](../resources/rolepermission.md) collection||
|isBuiltInRoleDefinition|Boolean||
|isBuiltIn|Boolean||
|roleScopeTagIds|String collection||



## Response
If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/roledefinition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_roledefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 828

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission"
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roledefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 877

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "8693b9d5-b9d5-8693-d5b9-9386d5b99386",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission"
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

