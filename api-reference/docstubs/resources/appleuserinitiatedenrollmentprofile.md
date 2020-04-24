---
title: "appleUserInitiatedEnrollmentProfile resource type"
description: "The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged. Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appleUserInitiatedEnrollmentProfile resource type


Namespace: microsoft.graph

The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged. Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get appleUserInitiatedEnrollmentProfile](../api/appleuserinitiatedenrollmentprofile-get.md)|[appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md)|Read the properties and relationships of an [appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) object.|
|[Update appleUserInitiatedEnrollmentProfile](../api/appleuserinitiatedenrollmentprofile-update.md)|[appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md)|Update the properties of an [appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) object.|
|[setPriority](../api/appleuserinitiatedenrollmentprofile-setpriority.md)|None|**TODO: Add Description**|
|[List assignments](../api/appleuserinitiatedenrollmentprofile-list-assignments.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) collection|Get the appleEnrollmentProfileAssignments from the assignments navigation property.|
|[Create assignments](../api/appleuserinitiatedenrollmentprofile-post-assignments.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/appleuserinitiatedenrollmentprofile-delete-assignments.md)|None|Delete an [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.|
|[Update assignments](../api/appleuserinitiatedenrollmentprofile-update-assignments.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Update the properties of an assignments object.|
|[Get appleEnrollmentProfileAssignment](../api/appleenrollmentprofileassignment-get.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Read the properties and relationships of an [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availableEnrollmentTypeOptions|[appleOwnerTypeEnrollmentType](../resources/appleownertypeenrollmenttype.md) collection|List of available enrollment type options|
|createdDateTime|DateTimeOffset|Profile creation time|
|defaultEnrollmentType|appleUserInitiatedEnrollmentType|The default profile enrollment type. Possible values are: `unknown`, `device`, `user`.|
|description|String|Description of the profile|
|displayName|String|Name of the profile|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Profile last modified time|
|platform|devicePlatformType|The platform of the Device. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|priority|Int32|Priority, 0 is highest|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) collection|The list of assignments for this profile.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "id": "String (identifier)",
  "defaultEnrollmentType": "String",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "String",
      "enrollmentType": "String"
    }
  ],
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "platform": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

