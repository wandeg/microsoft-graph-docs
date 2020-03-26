---
title: "accessPackage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackage resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackages](../api/accesspackage-list.md)|[accessPackage](../resources/accesspackage.md) collection|List properties and relationships of the [accessPackage](../resources/accesspackage.md) objects.|
|[Get accessPackage](../api/accesspackage-get.md)|[accessPackage](../resources/accesspackage.md)|Read properties and relationships of the [accessPackage](../resources/accesspackage.md) object.|
|[Create accessPackage](../api/accesspackage-post-accesspackages.md)|[accessPackage](../resources/accesspackage.md)|Create a new [accessPackage](../resources/accesspackage.md) object.|
|[Delete accessPackage](../api/accesspackage-delete.md)|None|Deletes a [accessPackage](../resources/accesspackage.md).|
|[Update accessPackage](../api/accesspackage-update.md)|[accessPackage](../resources/accesspackage.md)|Update the properties of a [accessPackage](../resources/accesspackage.md) object.|
|[Search](../api/accesspackage-search.md)|[accessPackage](../resources/accesspackage.md) collection||
|[Get accessPackageCatalog](../api/accesspackagecatalog-get.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Read properties and relationships of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[List accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md)|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) collection|Get the accessPackageResourceRoleScopes from the accessPackageResourceRoleScopes navigation property.|
|[Add accessPackageResourceRoleScopes](../api/accesspackage-post-accesspackageresourcerolescopes.md)|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)|Add accessPackageResourceRoleScopes by posting to the accessPackageResourceRoleScopes collection.|
|[List accessPackageAssignmentPolicies](../api/accesspackage-list-accesspackageassignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) collection|Get the accessPackageAssignmentPolicies from the accessPackageAssignmentPolicies navigation property.|
|[Add accessPackageAssignmentPolicies](../api/accesspackage-post-accesspackageassignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Add accessPackageAssignmentPolicies by posting to the accessPackageAssignmentPolicies collection.|
|[List accessPackages](../api/accesspackagecatalog-list-accesspackages.md)|[accessPackage](../resources/accesspackage.md) collection|Get the accessPackages from the accessPackages navigation property.|
|[Add accessPackages](../api/accesspackagecatalog-post-accesspackages.md)|[accessPackage](../resources/accesspackage.md)|Add accessPackages by posting to the accessPackages collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|catalogId|String||
|createdBy|String||
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isHidden|Boolean||
|isRoleScopesVisible|Boolean||
|modifiedBy|String||
|modifiedDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageAssignmentPolicies|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) collection||
|accessPackageCatalog|[accessPackageCatalog](../resources/accesspackagecatalog.md)||
|accessPackageResourceRoleScopes|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackage",
  "id": "String (identifier)",
  "catalogId": "String",
  "displayName": "String",
  "description": "String",
  "isHidden": true,
  "isRoleScopesVisible": true,
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

