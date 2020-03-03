---
title: "appleEnrollmentProfileAssignment resource type"
description: "An assignment of an Apple profile."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appleEnrollmentProfileAssignment resource type


Namespace: microsoft.graph

An assignment of an Apple profile.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List appleEnrollmentProfileAssignments](../api/appleenrollmentprofileassignment-list.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) collection|List properties and relationships of the [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) objects.|
|[Get appleEnrollmentProfileAssignment](../api/appleenrollmentprofileassignment-get.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Read properties and relationships of the [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.|
|[Create appleEnrollmentProfileAssignment](../api/appleenrollmentprofileassignment-create.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Create a new [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.|
|[Delete appleEnrollmentProfileAssignment](../api/appleenrollmentprofileassignment-delete.md)|None|Deletes a [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md).|
|[Update appleEnrollmentProfileAssignment](../api/appleenrollmentprofileassignment-update.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Update the properties of a [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceandappmanagementassignmenttarget.md)|The assignment target for the Apple user initiated deployment profile.|

## Relationships
None

## JSON Representation
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

