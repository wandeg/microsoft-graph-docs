---
title: "appleUserInitiatedEnrollmentProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appleUserInitiatedEnrollmentProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[setPriority](../api/appleuserinitiatedenrollmentprofile-setpriority.md)|None|**TODO: Add Description**|
|[List assignments](../api/appleuserinitiatedenrollmentprofile-list-assignments.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) collection|Get the appleEnrollmentProfileAssignments from the assignments navigation property.|
|[Create assignments](../api/appleuserinitiatedenrollmentprofile-post-assignments.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/appleuserinitiatedenrollmentprofile-delete-assignments.md)|None|Delete an [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.|
|[Update assignments](../api/appleuserinitiatedenrollmentprofile-update-assignments.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Update the properties of an assignments object.|
|[Get appleEnrollmentProfileAssignment](../api/appleenrollmentprofileassignment-get.md)|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md)|Read the properties and relationships of an [appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availableEnrollmentTypeOptions|[appleOwnerTypeEnrollmentType](../resources/appleownertypeenrollmenttype.md) collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|defaultEnrollmentType|appleUserInitiatedEnrollmentType|**TODO: Add Description**. Possible values are: `unknown`, `device`, `user`.|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|platform|devicePlatformType|**TODO: Add Description**. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|priority|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[appleEnrollmentProfileAssignment](../resources/appleenrollmentprofileassignment.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType"
    }
  ],
  "displayName": "String",
  "description": "String",
  "priority": "Integer",
  "platform": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

