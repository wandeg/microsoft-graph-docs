---
title: "windowsAutopilotDeviceIdentity resource type"
description: "The windowsAutopilotDeviceIdentity resource represents a Windows Autopilot Device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsAutopilotDeviceIdentity resource type


Namespace: microsoft.graph

The windowsAutopilotDeviceIdentity resource represents a Windows Autopilot Device.


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
|addressableUserName|String|Addressable user name.|
|azureActiveDirectoryDeviceId|String|AAD Device ID|
|deploymentProfileAssignedDateTime|DateTimeOffset|Profile set time of the Windows autopilot device.|
|deploymentProfileAssignmentDetailedStatus|Enumeration|Profile assignment detailed status of the Windows autopilot device. Possible values are: `none`, `hardwareRequirementsNotMet`.|
|deploymentProfileAssignmentStatus|Enumeration|Profile assignment status of the Windows autopilot device. Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.|
|displayName|String|Display Name|
|enrollmentState|Enumeration|Intune enrollment state of the Windows autopilot device. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|groupTag|String|Group Tag of the Windows autopilot device.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastContactedDateTime|DateTimeOffset|Intune Last Contacted Date Time of the Windows autopilot device.|
|managedDeviceId|String|Managed Device ID|
|manufacturer|String|Oem manufacturer of the Windows autopilot device.|
|model|String|Model name of the Windows autopilot device.|
|orderIdentifier|String|Order Identifier of the Windows autopilot device - Deprecated|
|productKey|String|Product Key of the Windows autopilot device.|
|purchaseOrderIdentifier|String|Purchase Order Identifier of the Windows autopilot device.|
|resourceName|String|Resource Name.|
|serialNumber|String|Serial number of the Windows autopilot device.|
|skuNumber|String|SKU Number|
|systemFamily|String|System Family|
|userPrincipalName|String|User Principal Name.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deploymentProfile|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|Deployment profile currently assigned to the Windows autopilot device.|
|intendedDeploymentProfile|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|Deployment profile intended to be assigned to the Windows autopilot device.|

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

