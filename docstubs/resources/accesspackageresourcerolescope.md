---
title: "accessPackageResourceRoleScope resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackageResourceRoleScope resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageResourceRoleScopes](../api/accesspackageresourcerolescope-list.md)|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) collection|List properties and relationships of the [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects.|
|[Get accessPackageResourceRoleScope](../api/accesspackageresourcerolescope-get.md)|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)|Read properties and relationships of the [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.|
|[Create accessPackageResourceRoleScope](../api/accesspackageresourcerolescope-post-accesspackageresourcerolescopes.md)|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)|Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.|
|[Delete accessPackageResourceRoleScope](../api/accesspackageresourcerolescope-delete.md)|None|Deletes a [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md).|
|[Update accessPackageResourceRoleScope](../api/accesspackageresourcerolescope-update.md)|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)|Update the properties of a [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.|
|[Get accessPackageResourceRole](../api/accesspackageresourcerole-get.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Read properties and relationships of the [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.|
|[Get accessPackageResourceScope](../api/accesspackageresourcescope-get.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Read properties and relationships of the [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[List accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md)|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) collection|Get the accessPackageResourceRoleScopes from the accessPackageResourceRoleScopes navigation property.|
|[Add accessPackageResourceRoleScopes](../api/accesspackage-post-accesspackageresourcerolescopes.md)|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)|Add accessPackageResourceRoleScopes by posting to the accessPackageResourceRoleScopes collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|String||
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|modifiedBy|String||
|modifiedDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageResourceRole|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)||
|accessPackageResourceScope|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
  "id": "String (identifier)",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

