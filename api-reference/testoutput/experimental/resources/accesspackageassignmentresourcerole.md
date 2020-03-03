---
title: "accessPackageAssignmentResourceRole resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# accessPackageAssignmentResourceRole resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md)|[accessPackageAssignmentResourceRole](../resources/accessPackageAssignmentResourceRole.md)|Read properties and relationships of the [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.|
|[Delete accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-delete.md)|None|Deletes a [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md).|
|[Update accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-update.md)|[accessPackageAssignmentResourceRole](../resources/accessPackageAssignmentResourceRole.md)|Update the properties of a [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.|
|[My](../api/accesspackageassignmentresourcerole-my.md)|[accessPackageAssignmentResourceRole](../resources/accessPackageAssignmentResourceRole.md) collection||
|[Get accessPackageResourceScope](../api/accesspackageresourcescope-get.md)|[accessPackageResourceScope](../resources/accessPackageResourceScope.md)|Read properties and relationships of the [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|
|[Get accessPackageResourceRole](../api/accesspackageresourcerole-get.md)|[accessPackageResourceRole](../resources/accessPackageResourceRole.md)|Read properties and relationships of the [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object.|
|[Get accessPackageSubject](../api/accesspackagesubject-get.md)|[accessPackageSubject](../resources/accessPackageSubject.md)|Read properties and relationships of the [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[List accessPackageAssignments](../api/accesspackageassignmentresourcerole-list-accesspackageassignments.md)|[accessPackageAssignment](../resources/accessPackageAssignment.md) collection|Get the accessPackageAssignments from the accessPackageAssignments navigation property.|
|[Add accessPackageAssignments](../api/accesspackageassignmentresourcerole-post-accesspackageassignments.md)|[accessPackageAssignment](../resources/accessPackageAssignment.md)|Add accessPackageAssignments by posting to the accessPackageAssignments collection.|
|[List accessPackageAssignmentResourceRoles](../api/accesspackageassignment-list-accesspackageassignmentresourceroles.md)|[accessPackageAssignmentResourceRole](../resources/accessPackageAssignmentResourceRole.md) collection|Get the accessPackageAssignmentResourceRoles from the accessPackageAssignmentResourceRoles navigation property.|
|[Add accessPackageAssignmentResourceRoles](../api/accesspackageassignment-post-accesspackageassignmentresourceroles.md)|[accessPackageAssignmentResourceRole](../resources/accessPackageAssignmentResourceRole.md)|Add accessPackageAssignmentResourceRoles by posting to the accessPackageAssignmentResourceRoles collection.|

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
|accessPackageAssignments|[accessPackageAssignment](../resources/accessPackageAssignment.md) collection||
|accessPackageResourceRole|[accessPackageResourceRole](../resources/accessPackageResourceRole.md)||
|accessPackageResourceScope|[accessPackageResourceScope](../resources/accessPackageResourceScope.md)||
|accessPackageSubject|[accessPackageSubject](../resources/accessPackageSubject.md)||

## JSON Representation
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

