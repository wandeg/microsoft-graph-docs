---
title: "accessPackageCatalog resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackageCatalog resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageCatalogs](../api/accesspackagecatalog-list.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md) collection|List properties and relationships of the [accessPackageCatalog](../resources/accesspackagecatalog.md) objects.|
|[Get accessPackageCatalog](../api/accesspackagecatalog-get.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Read properties and relationships of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Create accessPackageCatalog](../api/accesspackagecatalog-post-accesspackagecatalogs.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Delete accessPackageCatalog](../api/accesspackagecatalog-delete.md)|None|Deletes a [accessPackageCatalog](../resources/accesspackagecatalog.md).|
|[Update accessPackageCatalog](../api/accesspackagecatalog-update.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Update the properties of a [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Search](../api/accesspackagecatalog-search.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md) collection||
|[List accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md)|[accessPackageResource](../resources/accesspackageresource.md) collection|Get the accessPackageResources from the accessPackageResources navigation property.|
|[Add accessPackageResources](../api/accesspackagecatalog-post-accesspackageresources.md)|[accessPackageResource](../resources/accesspackageresource.md)|Add accessPackageResources by posting to the accessPackageResources collection.|
|[List accessPackageResourceRoles](../api/accesspackagecatalog-list-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection|Get the accessPackageResourceRoles from the accessPackageResourceRoles navigation property.|
|[Add accessPackageResourceRoles](../api/accesspackagecatalog-post-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Add accessPackageResourceRoles by posting to the accessPackageResourceRoles collection.|
|[List accessPackageResourceScopes](../api/accesspackagecatalog-list-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md) collection|Get the accessPackageResourceScopes from the accessPackageResourceScopes navigation property.|
|[Add accessPackageResourceScopes](../api/accesspackagecatalog-post-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Add accessPackageResourceScopes by posting to the accessPackageResourceScopes collection.|
|[List accessPackages](../api/accesspackagecatalog-list-accesspackages.md)|[accessPackage](../resources/accesspackage.md) collection|Get the accessPackages from the accessPackages navigation property.|
|[Add accessPackages](../api/accesspackagecatalog-post-accesspackages.md)|[accessPackage](../resources/accesspackage.md)|Add accessPackages by posting to the accessPackages collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|catalogStatus|String||
|catalogType|String||
|createdBy|String||
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isExternallyVisible|Boolean||
|modifiedBy|String||
|modifiedDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageResourceRoles|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection||
|accessPackageResources|[accessPackageResource](../resources/accesspackageresource.md) collection||
|accessPackageResourceScopes|[accessPackageResourceScope](../resources/accesspackageresourcescope.md) collection||
|accessPackages|[accessPackage](../resources/accesspackage.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "catalogType": "String",
  "catalogStatus": "String",
  "isExternallyVisible": true,
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

