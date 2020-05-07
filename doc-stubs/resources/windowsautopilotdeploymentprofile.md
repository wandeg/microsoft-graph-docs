---
title: "windowsAutopilotDeploymentProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsAutopilotDeploymentProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[hasPayloadLinks](../api/windowsautopilotdeploymentprofile-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection|**TODO: Add Description**|
|[assign](../api/windowsautopilotdeploymentprofile-assign.md)|None|**TODO: Add Description**|
|[List assignedDevices](../api/windowsautopilotdeploymentprofile-list-assigneddevices.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) collection|Get the windowsAutopilotDeviceIdentities from the assignedDevices navigation property.|
|[Create assignedDevices](../api/windowsautopilotdeploymentprofile-post-assigneddevices.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Create a new assignedDevices object.|
|[Delete assignedDevices](../api/windowsautopilotdeploymentprofile-delete-assigneddevices.md)|None|Delete an [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) object.|
|[Update assignedDevices](../api/windowsautopilotdeploymentprofile-update-assigneddevices.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Update the properties of an assignedDevices object.|
|[Get windowsAutopilotDeviceIdentity](../api/windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Read the properties and relationships of a [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) object.|
|[List assignments](../api/windowsautopilotdeploymentprofile-list-assignments.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/windowsautopilotdeploymentprofileassignment.md) collection|Get the windowsAutopilotDeploymentProfileAssignments from the assignments navigation property.|
|[Create assignments](../api/windowsautopilotdeploymentprofile-post-assignments.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/windowsautopilotdeploymentprofileassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/windowsautopilotdeploymentprofile-delete-assignments.md)|None|Delete an [windowsAutopilotDeploymentProfileAssignment](../resources/windowsautopilotdeploymentprofileassignment.md) object.|
|[Update assignments](../api/windowsautopilotdeploymentprofile-update-assignments.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/windowsautopilotdeploymentprofileassignment.md)|Update the properties of an assignments object.|
|[Get windowsAutopilotDeploymentProfileAssignment](../api/windowsautopilotdeploymentprofileassignment-get.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/windowsautopilotdeploymentprofileassignment.md)|Read the properties and relationships of a [windowsAutopilotDeploymentProfileAssignment](../resources/windowsautopilotdeploymentprofileassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|deviceNameTemplate|String|**TODO: Add Description**|
|deviceType|windowsAutopilotDeviceType|**TODO: Add Description**. Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.|
|displayName|String|**TODO: Add Description**|
|enableWhiteGlove|Boolean|**TODO: Add Description**|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/windowsenrollmentstatusscreensettings.md)|**TODO: Add Description**|
|extractHardwareHash|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|language|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/outofboxexperiencesettings.md)|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignedDevices|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) collection|**TODO: Add Description**|
|assignments|[windowsAutopilotDeploymentProfileAssignment](../resources/windowsautopilotdeploymentprofileassignment.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
  },
  "extractHardwareHash": "Boolean",
  "deviceNameTemplate": "String",
  "deviceType": "String",
  "enableWhiteGlove": "Boolean",
  "roleScopeTagIds": [
    "String"
  ]
}
```

