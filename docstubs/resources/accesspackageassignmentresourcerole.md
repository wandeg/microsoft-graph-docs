---
title: "accessPackageAssignmentResourceRole resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackageAssignmentResourceRole resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md)|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) collection|List properties and relationships of the [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects.|
|[Get accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md)|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)|Read properties and relationships of the [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.|
|[Create accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-post-accesspackageassignmentresourceroles.md)|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)|Create a new [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.|
|[Delete accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-delete.md)|None|Deletes a [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md).|
|[Update accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-update.md)|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)|Update the properties of a [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.|
|[My](../api/accesspackageassignmentresourcerole-my.md)|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) collection||
|[Get accessPackageResourceScope](../api/accesspackageresourcescope-get.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Read properties and relationships of the [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[Get accessPackageResourceRole](../api/accesspackageresourcerole-get.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|Read properties and relationships of the [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.|
|[Get accessPackageSubject](../api/accesspackagesubject-get.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Read properties and relationships of the [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[List accessPackageAssignments](../api/accesspackageassignmentresourcerole-list-accesspackageassignments.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) collection|Get the accessPackageAssignments from the accessPackageAssignments navigation property.|
|[Add accessPackageAssignments](../api/accesspackageassignmentresourcerole-post-accesspackageassignments.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Add accessPackageAssignments by posting to the accessPackageAssignments collection.|
|[List accessPackageAssignmentResourceRoles](../api/accesspackageassignment-list-accesspackageassignmentresourceroles.md)|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) collection|Get the accessPackageAssignmentResourceRoles from the accessPackageAssignmentResourceRoles navigation property.|
|[Add accessPackageAssignmentResourceRoles](../api/accesspackageassignment-post-accesspackageassignmentresourceroles.md)|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)|Add accessPackageAssignmentResourceRoles by posting to the accessPackageAssignmentResourceRoles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|originId|String||
|originSystem|String||
|status|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageAssignments|[accessPackageAssignment](../resources/accesspackageassignment.md) collection||
|accessPackageResourceRole|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)||
|accessPackageResourceScope|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)||
|accessPackageSubject|[accessPackageSubject](../resources/accesspackagesubject.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentResourceRole",
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String",
  "status": "String"
}
```

