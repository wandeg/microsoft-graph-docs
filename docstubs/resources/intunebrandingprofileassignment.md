---
title: "intuneBrandingProfileAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# intuneBrandingProfileAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get intuneBrandingProfileAssignment](../api/intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Read properties and relationships of the [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) object.|
|[Update intuneBrandingProfileAssignment](../api/intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Update the properties of a [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) object.|
|[List assignments](../api/intunebrandingprofile-list-assignments.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) collection|Get the intuneBrandingProfileAssignments from the assignments navigation property.|
|[Add assignments](../api/intunebrandingprofile-post-assignments.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Add assignments by posting to the assignments collection.|

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
  "@odata.type": "microsoft.graph.intuneBrandingProfileAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

