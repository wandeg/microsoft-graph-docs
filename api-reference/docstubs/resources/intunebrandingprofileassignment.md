---
title: "intuneBrandingProfileAssignment resource type"
description: "This entity contains the properties used to assign a branding profile to a group."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# intuneBrandingProfileAssignment resource type


Namespace: microsoft.graph

This entity contains the properties used to assign a branding profile to a group.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get intuneBrandingProfileAssignment](../api/intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Read the properties and relationships of an [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) object.|
|[Update intuneBrandingProfileAssignment](../api/intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md)|Update the properties of an [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|Assignment target that the branding profile is assigned to.|

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

