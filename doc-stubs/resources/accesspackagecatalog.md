---
title: "accessPackageCatalog resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageCatalog resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageCatalogs](../api/accesspackagecatalog-list.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md) collection|Get a list of the [accessPackageCatalog](../resources/accesspackagecatalog.md) objects and their properties.|
|[Get accessPackageCatalog](../api/accesspackagecatalog-get.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Read the properties and relationships of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Create accessPackageCatalog](../api/accesspackagecatalog-post-accesspackagecatalogs.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Create a new [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Delete accessPackageCatalog](../api/accesspackagecatalog-delete.md)|None|Deletes an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Update accessPackageCatalog](../api/accesspackagecatalog-update.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Update the properties of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[Search](../api/accesspackagecatalog-search.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md) collection|**TODO: Add Description**|
|[List accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md)|[accessPackageResource](../resources/accesspackageresource.md) collection|Get the accessPackageResources from the accessPackageResources navigation property.|
|[Create accessPackageResources](../api/accesspackagecatalog-post-accesspackageresources.md)|[accessPackageResource](../resources/accesspackageresource.md)|Create a new accessPackageResources object.|
|[Delete accessPackageResources](../api/accesspackagecatalog-delete-accesspackageresources.md)|None|Delete an [accessPackageResource](../resources/accesspackageresource.md) object.|
|[Update accessPackageResources](../api/accesspackagecatalog-update-accesspackageresources.md)|[accessPackageResource](../resources/accesspackageresource.md)|Update the properties of an accessPackageResources object.|
|[Get accessPackageResource](../api/accesspackageresource-get.md)|[accessPackageResource](../resources/accesspackageresource.md)|Read the properties and relationships of an [accessPackageResource](../resources/accesspackageresource.md) object.|
|[List accessPackageResourceRoles](../api/accesspackagecatalog-list-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection|Get the accessPackageResourceRoles from the accessPackageResourceRoles navigation property.|
|[Create accessPackageResourceRoles](../api/accesspackagecatalog-post-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Create a new accessPackageResourceRoles object.|
|[Delete accessPackageResourceRoles](../api/accesspackagecatalog-delete-accesspackageresourceroles.md)|None|Delete an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.|
|[Update accessPackageResourceRoles](../api/accesspackagecatalog-update-accesspackageresourceroles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Update the properties of an accessPackageResourceRoles object.|
|[Get accessPackageResourceRole](../api/accesspackageresourcerole-get.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Read the properties and relationships of an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.|
|[List accessPackageResourceScopes](../api/accesspackagecatalog-list-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md) collection|Get the accessPackageResourceScopes from the accessPackageResourceScopes navigation property.|
|[Create accessPackageResourceScopes](../api/accesspackagecatalog-post-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Create a new accessPackageResourceScopes object.|
|[Delete accessPackageResourceScopes](../api/accesspackagecatalog-delete-accesspackageresourcescopes.md)|None|Delete an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[Update accessPackageResourceScopes](../api/accesspackagecatalog-update-accesspackageresourcescopes.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Update the properties of an accessPackageResourceScopes object.|
|[Get accessPackageResourceScope](../api/accesspackageresourcescope-get.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Read the properties and relationships of an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[List accessPackages](../api/accesspackagecatalog-list-accesspackages.md)|[accessPackage](../resources/accesspackage.md) collection|Get the accessPackages from the accessPackages navigation property.|
|[Create accessPackages](../api/accesspackagecatalog-post-accesspackages.md)|[accessPackage](../resources/accesspackage.md)|Create a new accessPackages object.|
|[Delete accessPackages](../api/accesspackagecatalog-delete-accesspackages.md)|None|Delete an [accessPackage](../resources/accesspackage.md) object.|
|[Update accessPackages](../api/accesspackagecatalog-update-accesspackages.md)|[accessPackage](../resources/accesspackage.md)|Update the properties of an accessPackages object.|
|[Get accessPackage](../api/accesspackage-get.md)|[accessPackage](../resources/accesspackage.md)|Read the properties and relationships of an [accessPackage](../resources/accesspackage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|catalogStatus|String|**TODO: Add Description**|
|catalogType|String|**TODO: Add Description**|
|createdBy|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isExternallyVisible|Boolean|**TODO: Add Description**|
|modifiedBy|String|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageResourceRoles|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection|**TODO: Add Description**|
|accessPackageResources|[accessPackageResource](../resources/accesspackageresource.md) collection|**TODO: Add Description**|
|accessPackageResourceScopes|[accessPackageResourceScope](../resources/accesspackageresourcescope.md) collection|**TODO: Add Description**|
|accessPackages|[accessPackage](../resources/accesspackage.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "isExternallyVisible": "Boolean",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

