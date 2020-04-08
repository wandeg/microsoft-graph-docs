---
title: "windowsAutopilotDeploymentProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsAutopilotDeploymentProfile resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsAutopilotDeploymentProfile](../api/windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) object.|
|[hasPayloadLinks](../api/windowsautopilotdeploymentprofile-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection||
|[assign](../api/windowsautopilotdeploymentprofile-assign.md)|None||
|[List assignedDevices](../api/windowsautopilotdeploymentprofile-list-assigneddevices.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) collection|Get the windowsAutopilotDeviceIdentities from the assignedDevices navigation property.|
|[Add assignedDevices](../api/windowsautopilotdeploymentprofile-post-assigneddevices.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Add assignedDevices by posting to the assignedDevices collection.|
|[List assignments](../api/windowsautopilotdeploymentprofile-list-assignments.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/windowsautopilotdeploymentprofileassignment.md) collection|Get the windowsAutopilotDeploymentProfileAssignments from the assignments navigation property.|
|[Add assignments](../api/windowsautopilotdeploymentprofile-post-assignments.md)|[windowsAutopilotDeploymentProfileAssignment](../resources/windowsautopilotdeploymentprofileassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|description|String||
|deviceNameTemplate|String||
|deviceType|Enumeration| Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.|
|displayName|String||
|enableWhiteGlove|Boolean||
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/windowsenrollmentstatusscreensettings.md)||
|extractHardwareHash|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|language|String||
|lastModifiedDateTime|DateTimeOffset||
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/outofboxexperiencesettings.md)||
|roleScopeTagIds|String collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignedDevices|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) collection||
|assignments|[windowsAutopilotDeploymentProfileAssignment](../resources/windowsautopilotdeploymentprofileassignment.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "String",
    "deviceUsageType": "String",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "String",
    "installProgressTimeoutInMinutes": 1024,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "String",
  "deviceType": "String",
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```

