---
title: "windowsFeatureUpdateProfile resource type"
description: "Windows Feature Update Profile"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsFeatureUpdateProfile resource type

Windows Feature Update Profile


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsFeatureUpdateProfile](../api/windowsfeatureupdateprofile-get.md)|[windowsFeatureUpdateProfile](../resources/windowsFeatureUpdateProfile.md)|Read properties and relationships of the [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) object.|
|[Delete windowsFeatureUpdateProfile](../api/windowsfeatureupdateprofile-delete.md)|None|Deletes a [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md).|
|[Update windowsFeatureUpdateProfile](../api/windowsfeatureupdateprofile-update.md)|[windowsFeatureUpdateProfile](../resources/windowsFeatureUpdateProfile.md)|Update the properties of a [windowsFeatureUpdateProfile](../resources/windowsfeatureupdateprofile.md) object.|
|[assign](../api/windowsfeatureupdateprofile-assign.md)|None||
|[List assignments](../api/windowsfeatureupdateprofile-list-assignments.md)|[windowsFeatureUpdateProfileAssignment](../resources/windowsFeatureUpdateProfileAssignment.md) collection|Get the windowsFeatureUpdateProfileAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsfeatureupdateprofile-post-assignments.md)|[windowsFeatureUpdateProfileAssignment](../resources/windowsFeatureUpdateProfileAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceUpdateStates](../api/windowsfeatureupdateprofile-list-deviceupdatestates.md)|[windowsUpdateState](../resources/windowsUpdateState.md) collection|Get the windowsUpdateStates from the deviceUpdateStates navigation property.|
|[Add deviceUpdateStates](../api/windowsfeatureupdateprofile-post-deviceupdatestates.md)|[windowsUpdateState](../resources/windowsUpdateState.md)|Add deviceUpdateStates by posting to the deviceUpdateStates collection.|
|[List windowsFeatureUpdateProfiles](../api/intune-devices-devicemanagement-list-windowsfeatureupdateprofiles.md)|[windowsFeatureUpdateProfile](../resources/windowsFeatureUpdateProfile.md) collection|Get the windowsFeatureUpdateProfiles from the windowsFeatureUpdateProfiles navigation property.|
|[Add windowsFeatureUpdateProfiles](../api/intune-devices-devicemanagement-post-windowsfeatureupdateprofiles.md)|[windowsFeatureUpdateProfile](../resources/windowsFeatureUpdateProfile.md)|Add windowsFeatureUpdateProfiles by posting to the windowsFeatureUpdateProfiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date time that the profile was created.|
|description|String|The description of the profile which is specified by the user.|
|displayName|String|The display name of the profile.|
|featureUpdateVersion|String|The feature update version that will be deployed to the devices targeted by this profile. The version could be any supported version for example 1709, 1803 or 1809 and so on.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date time that the profile was last modified.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[windowsFeatureUpdateProfileAssignment](../resources/windowsFeatureUpdateProfileAssignment.md) collection|The list of group assignments of the profile.|
|deviceUpdateStates|[windowsUpdateState](../resources/windowsUpdateState.md) collection|The list of device states this profile targeted to|

## JSON Representation
Here is a JSON representation of the resource.
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

