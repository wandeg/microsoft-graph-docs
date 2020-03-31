---
title: "windowsAutopilotDeviceIdentity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsAutopilotDeviceIdentity resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsAutopilotDeviceIdentity](../api/windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Read properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) object.|
|[Update windowsAutopilotDeviceIdentity](../api/windowsautopilotdeviceidentity-update.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Update the properties of a [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) object.|
|[assignUserToDevice](../api/windowsautopilotdeviceidentity-assignusertodevice.md)|None||
|[unassignUserFromDevice](../api/windowsautopilotdeviceidentity-unassignuserfromdevice.md)|None||
|[updateDeviceProperties](../api/windowsautopilotdeviceidentity-updatedeviceproperties.md)|None||
|[assignResourceAccountToDevice](../api/windowsautopilotdeviceidentity-assignresourceaccounttodevice.md)|None||
|[unassignResourceAccountFromDevice](../api/windowsautopilotdeviceidentity-unassignresourceaccountfromdevice.md)|None||
|[Get windowsAutopilotDeploymentProfile](../api/windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) object.|
|[Get windowsAutopilotDeploymentProfile](../api/windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) object.|
|[List assignedDevices](../api/windowsautopilotdeploymentprofile-list-assigneddevices.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) collection|Get the windowsAutopilotDeviceIdentities from the assignedDevices navigation property.|
|[Add assignedDevices](../api/windowsautopilotdeploymentprofile-post-assigneddevices.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Add assignedDevices by posting to the assignedDevices collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addressableUserName|String||
|azureActiveDirectoryDeviceId|String||
|deploymentProfileAssignedDateTime|DateTimeOffset||
|deploymentProfileAssignmentDetailedStatus|Enumeration| Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.|
|deploymentProfileAssignmentStatus|Enumeration| Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.|
|displayName|String||
|enrollmentState|Enumeration| Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|groupTag|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastContactedDateTime|DateTimeOffset||
|managedDeviceId|String||
|manufacturer|String||
|model|String||
|orderIdentifier|String||
|productKey|String||
|purchaseOrderIdentifier|String||
|resourceName|String||
|serialNumber|String||
|skuNumber|String||
|systemFamily|String||
|userPrincipalName|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deploymentProfile|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)||
|intendedDeploymentProfile|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeviceIdentity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "deploymentProfileAssignmentStatus": "String",
  "deploymentProfileAssignmentDetailedStatus": "String",
  "deploymentProfileAssignedDateTime": "String (timestamp)",
  "orderIdentifier": "String",
  "groupTag": "String",
  "purchaseOrderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "manufacturer": "String",
  "model": "String",
  "enrollmentState": "String",
  "lastContactedDateTime": "String (timestamp)",
  "addressableUserName": "String",
  "userPrincipalName": "String",
  "resourceName": "String",
  "skuNumber": "String",
  "systemFamily": "String",
  "azureActiveDirectoryDeviceId": "String",
  "managedDeviceId": "String",
  "displayName": "String"
}
```

