---
title: "accessPackageCatalog resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# accessPackageCatalog resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageCatalogs](../api/accesspackagecatalog-list.md)|[accessPackageCatalog](../resources/accessPackageCatalog.md) collection|List properties and relationships of the [accessPackageCatalog](../resources/accesspackagecatalog.md) objects.|
|[Get accessPackageCatalog](../api/accesspackagecatalog-get.md)|[accessPackageCatalog](../resources/accessPackageCatalog.md)|Read properties and relationships of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Create accessPackageCatalog](../api/accesspackagecatalog-post-accesspackagecatalogs.md)|[accessPackageCatalog](../resources/accessPackageCatalog.md)|Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Delete accessPackageCatalog](../api/accesspackagecatalog-delete.md)|None|Deletes a [accessPackageCatalog](../resources/accesspackagecatalog.md).|
|[Update accessPackageCatalog](../api/accesspackagecatalog-update.md)|[accessPackageCatalog](../resources/accessPackageCatalog.md)|Update the properties of a [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Search](../api/accesspackagecatalog-search.md)|[accessPackageCatalog](../resources/accessPackageCatalog.md) collection||
|[List accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md)|[accessPackageResource](../resources/accessPackageResource.md) collection|Get the accessPackageResources from the accessPackageResources navigation property.|
|[Add accessPackageResources](../api/accesspackagecatalog-post-accesspackageresources.md)|[accessPackageResource](../resources/accessPackageResource.md)|Add accessPackageResources by posting to the accessPackageResources collection.|
|[List accessPackageResourceRoles](../api/accesspackagecatalog-list-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accessPackageResourceRole.md) collection|Get the accessPackageResourceRoles from the accessPackageResourceRoles navigation property.|
|[Add accessPackageResourceRoles](../api/accesspackagecatalog-post-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accessPackageResourceRole.md)|Add accessPackageResourceRoles by posting to the accessPackageResourceRoles collection.|
|[List accessPackageResourceScopes](../api/accesspackagecatalog-list-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accessPackageResourceScope.md) collection|Get the accessPackageResourceScopes from the accessPackageResourceScopes navigation property.|
|[Add accessPackageResourceScopes](../api/accesspackagecatalog-post-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accessPackageResourceScope.md)|Add accessPackageResourceScopes by posting to the accessPackageResourceScopes collection.|
|[List accessPackages](../api/accesspackagecatalog-list-accesspackages.md)|[accessPackage](../resources/accessPackage.md) collection|Get the accessPackages from the accessPackages navigation property.|
|[Add accessPackages](../api/accesspackagecatalog-post-accesspackages.md)|[accessPackage](../resources/accessPackage.md)|Add accessPackages by posting to the accessPackages collection.|

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
|accessPackageResourceRoles|[accessPackageResourceRole](../resources/accessPackageResourceRole.md) collection||
|accessPackageResources|[accessPackageResource](../resources/accessPackageResource.md) collection||
|accessPackageResourceScopes|[accessPackageResourceScope](../resources/accessPackageResourceScope.md) collection||
|accessPackages|[accessPackage](../resources/accessPackage.md) collection||

## JSON Representation
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

