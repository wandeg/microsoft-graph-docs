---
title: "intuneBrandingProfileAssignment resource type"
description: "This entity contains the properties used to assign a branding profile to a group."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# intuneBrandingProfileAssignment resource type


Namespace: microsoft.graph

This entity contains the properties used to assign a branding profile to a group.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List intuneBrandingProfileAssignments](../api/intunebrandingprofileassignment-list.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) collection|List properties and relationships of the [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) objects.|
|[Get intuneBrandingProfileAssignment](../api/intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Read properties and relationships of the [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) object.|
|[Create intuneBrandingProfileAssignment](../api/intunebrandingprofileassignment-create.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Create a new [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) object.|
|[Delete intuneBrandingProfileAssignment](../api/intunebrandingprofileassignment-delete.md)|None|Deletes a [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md).|
|[Update intuneBrandingProfileAssignment](../api/intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Update the properties of a [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceandappmanagementassignmenttarget.md)|Assignment target that the branding profile is assigned to.|

## Relationships
None

## JSON Representation
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

