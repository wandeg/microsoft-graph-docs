---
title: "accessPackageAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessPackageAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessPackageAssignments](../api/accesspackageassignment-list.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) collection|List properties and relationships of the [accessPackageAssignment](../resources/accesspackageassignment.md) objects.|
|[Get accessPackageAssignment](../api/accesspackageassignment-get.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Read properties and relationships of the [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[Create accessPackageAssignment](../api/accesspackageassignment-post-accesspackageassignments.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Create a new [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[Delete accessPackageAssignment](../api/accesspackageassignment-delete.md)|None|Deletes a [accessPackageAssignment](../resources/accesspackageassignment.md).|
|[Update accessPackageAssignment](../api/accesspackageassignment-update.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Update the properties of a [accessPackageAssignment](../resources/accesspackageassignment.md) object.|
|[My](../api/accesspackageassignment-my.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) collection||
|[Get accessPackage](../api/accesspackage-get.md)|[accessPackage](../resources/accesspackage.md)|Read properties and relationships of the [accessPackage](../resources/accesspackage.md) object.|
|[Get accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Read properties and relationships of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.|
|[Get accessPackageSubject](../api/accesspackagesubject-get.md)|[accessPackageSubject](../resources/accesspackagesubject.md)|Read properties and relationships of the [accessPackageSubject](../resources/accesspackagesubject.md) object.|
|[List accessPackageAssignmentRequests](../api/accesspackageassignment-list-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection|Get the accessPackageAssignmentRequests from the accessPackageAssignmentRequests navigation property.|
|[Add accessPackageAssignmentRequests](../api/accesspackageassignment-post-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Add accessPackageAssignmentRequests by posting to the accessPackageAssignmentRequests collection.|
|[List accessPackageAssignmentResourceRoles](../api/accesspackageassignment-list-accesspackageassignmentresourceroles.md)|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) collection|Get the accessPackageAssignmentResourceRoles from the accessPackageAssignmentResourceRoles navigation property.|
|[Add accessPackageAssignmentResourceRoles](../api/accesspackageassignment-post-accesspackageassignmentresourceroles.md)|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)|Add accessPackageAssignmentResourceRoles by posting to the accessPackageAssignmentResourceRoles collection.|
|[List accessPackageAssignments](../api/accesspackageassignmentresourcerole-list-accesspackageassignments.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) collection|Get the accessPackageAssignments from the accessPackageAssignments navigation property.|
|[Add accessPackageAssignments](../api/accesspackageassignmentresourcerole-post-accesspackageassignments.md)|[accessPackageAssignment](../resources/accesspackageassignment.md)|Add accessPackageAssignments by posting to the accessPackageAssignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessPackageId|String||
|assignmentPolicyId|String||
|assignmentState|String||
|assignmentStatus|String||
|catalogId|String||
|expiredDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|isExtended|Boolean||
|targetId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)||
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)||
|accessPackageAssignmentRequests|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection||
|accessPackageAssignmentResourceRoles|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) collection||
|target|[accessPackageSubject](../resources/accesspackagesubject.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "id": "String (identifier)",
  "catalogId": "String",
  "accessPackageId": "String",
  "assignmentPolicyId": "String",
  "targetId": "String",
  "assignmentStatus": "String",
  "assignmentState": "String",
  "isExtended": true,
  "expiredDateTime": "String (timestamp)"
}
```

