---
title: "unifiedRoleDefinition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# unifiedRoleDefinition resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get unifiedRoleDefinition](../api/unifiedroledefinition-get.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Read properties and relationships of the [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.|
|[Update unifiedRoleDefinition](../api/unifiedroledefinition-update.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isBuiltIn|Boolean||
|isEnabled|Boolean||
|resourceScopes|String collection||
|rolePermissions|[unifiedRolePermission](../resources/unifiedrolepermission.md) collection||
|templateId|String||
|version|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "isBuiltIn": true,
  "isEnabled": true,
  "resourceScopes": [
    "String"
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.unifiedRolePermission"
    }
  ],
  "templateId": "String",
  "version": "String"
}
```

