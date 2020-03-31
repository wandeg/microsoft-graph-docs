---
title: "appleEnrollmentProfileAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appleEnrollmentProfileAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get appleEnrollmentProfileAssignment](../api/appleenrollmentprofileassignment-get.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Read properties and relationships of the [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.|
|[Update appleEnrollmentProfileAssignment](../api/appleenrollmentprofileassignment-update.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Update the properties of a [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.|
|[List assignments](../api/appleuserinitiatedenrollmentprofile-list-assignments.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) collection|Get the appleEnrollmentProfileAssignments from the assignments navigation property.|
|[Add assignments](../api/appleuserinitiatedenrollmentprofile-post-assignments.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleEnrollmentProfileAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

