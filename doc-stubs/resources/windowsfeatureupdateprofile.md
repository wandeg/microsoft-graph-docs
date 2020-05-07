---
title: "windowsFeatureUpdateProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsFeatureUpdateProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[assign](../api/windowsfeatureupdateprofile-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/windowsfeatureupdateprofile-list-assignments.md)|[windowsFeatureUpdateProfileAssignment](../resources/windowsfeatureupdateprofileassignment.md) collection|Get the windowsFeatureUpdateProfileAssignments from the assignments navigation property.|
|[Create assignments](../api/windowsfeatureupdateprofile-post-assignments.md)|[windowsFeatureUpdateProfileAssignment](../resources/windowsfeatureupdateprofileassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/windowsfeatureupdateprofile-delete-assignments.md)|None|Delete an [windowsFeatureUpdateProfileAssignment](../resources/windowsfeatureupdateprofileassignment.md) object.|
|[Update assignments](../api/windowsfeatureupdateprofile-update-assignments.md)|[windowsFeatureUpdateProfileAssignment](../resources/windowsfeatureupdateprofileassignment.md)|Update the properties of an assignments object.|
|[Get windowsFeatureUpdateProfileAssignment](../api/windowsfeatureupdateprofileassignment-get.md)|[windowsFeatureUpdateProfileAssignment](../resources/windowsfeatureupdateprofileassignment.md)|Read the properties and relationships of a [windowsFeatureUpdateProfileAssignment](../resources/windowsfeatureupdateprofileassignment.md) object.|
|[List deviceUpdateStates](../api/windowsfeatureupdateprofile-list-deviceupdatestates.md)|[windowsUpdateState](../resources/windowsupdatestate.md) collection|Get the windowsUpdateStates from the deviceUpdateStates navigation property.|
|[Create deviceUpdateStates](../api/windowsfeatureupdateprofile-post-deviceupdatestates.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Create a new deviceUpdateStates object.|
|[Delete deviceUpdateStates](../api/windowsfeatureupdateprofile-delete-deviceupdatestates.md)|None|Delete a [windowsUpdateState](../resources/windowsupdatestate.md) object.|
|[Update deviceUpdateStates](../api/windowsfeatureupdateprofile-update-deviceupdatestates.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Update the properties of a deviceUpdateStates object.|
|[Get windowsUpdateState](../api/windowsupdatestate-get.md)|[windowsUpdateState](../resources/windowsupdatestate.md)|Read the properties and relationships of a [windowsUpdateState](../resources/windowsupdatestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|featureUpdateVersion|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[windowsFeatureUpdateProfileAssignment](../resources/windowsfeatureupdateprofileassignment.md) collection|**TODO: Add Description**|
|deviceUpdateStates|[windowsUpdateState](../resources/windowsupdatestate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFeatureUpdateProfile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "featureUpdateVersion": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

