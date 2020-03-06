---
title: "accessPackageAssignmentPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackageAssignmentPolicy resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) collection|List properties and relationships of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.|
|[Get accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Read properties and relationships of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.|
|[Create accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post-accesspackageassignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.|
|[Delete accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md)|None|Deletes a [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).|
|[Update accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Update the properties of a [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.|
|[Get accessPackage](../api/accesspackage-get.md)|[accessPackage](../resources/accesspackage.md)|Read properties and relationships of the [accessPackage](../resources/accesspackage.md) object.|
|[Get accessPackageCatalog](../api/accesspackagecatalog-get.md)|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Read properties and relationships of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.|
|[List accessPackageAssignmentPolicies](../api/accesspackage-list-accesspackageassignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) collection|Get the accessPackageAssignmentPolicies from the accessPackageAssignmentPolicies navigation property.|
|[Add accessPackageAssignmentPolicies](../api/accesspackage-post-accesspackageassignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Add accessPackageAssignmentPolicies by posting to the accessPackageAssignmentPolicies collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessPackageId|String||
|canExtend|Boolean||
|createdBy|String||
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|durationInDays|Int32||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|isEnabled|Boolean||
|modifiedBy|String||
|modifiedDateTime|DateTimeOffset||
|userType|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)||
|accessPackageCatalog|[accessPackageCatalog](../resources/accesspackagecatalog.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "id": "String (identifier)",
  "userType": "String",
  "accessPackageId": "String",
  "displayName": "String",
  "description": "String",
  "isEnabled": true,
  "canExtend": true,
  "durationInDays": 1024,
  "expirationDateTime": "String (timestamp)",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

