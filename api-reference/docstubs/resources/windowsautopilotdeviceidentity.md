---
title: "windowsAutopilotDeviceIdentity resource type"
description: "The windowsAutopilotDeviceIdentity resource represents a Windows Autopilot Device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsAutopilotDeviceIdentity resource type


Namespace: microsoft.graph

The windowsAutopilotDeviceIdentity resource represents a Windows Autopilot Device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsAutopilotDeviceIdentity](../api/windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Read the properties and relationships of a [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) object.|
|[Update windowsAutopilotDeviceIdentity](../api/windowsautopilotdeviceidentity-update.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Update the properties of a [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) object.|
|[assignUserToDevice](../api/windowsautopilotdeviceidentity-assignusertodevice.md)|None|**TODO: Add Description**|
|[unassignUserFromDevice](../api/windowsautopilotdeviceidentity-unassignuserfromdevice.md)|None|**TODO: Add Description**|
|[updateDeviceProperties](../api/windowsautopilotdeviceidentity-updatedeviceproperties.md)|None|**TODO: Add Description**|
|[assignResourceAccountToDevice](../api/windowsautopilotdeviceidentity-assignresourceaccounttodevice.md)|None|**TODO: Add Description**|
|[unassignResourceAccountFromDevice](../api/windowsautopilotdeviceidentity-unassignresourceaccountfromdevice.md)|None|**TODO: Add Description**|
|[List deploymentProfile](../api/windowsautopilotdeviceidentity-list-deploymentprofile.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) collection|Get the windowsAutopilotDeploymentProfiles from the deploymentProfile navigation property.|
|[Add deploymentProfile](../api/windowsautopilotdeviceidentity-post-deploymentprofile.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|Add deploymentProfile by posting to the deploymentProfile collection.|
|[Remove deploymentProfile](../api/windowsautopilotdeviceidentity-delete-deploymentprofile.md)|None|Remove a [windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) object.|
|[List intendedDeploymentProfile](../api/windowsautopilotdeviceidentity-list-intendeddeploymentprofile.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) collection|Get the windowsAutopilotDeploymentProfiles from the intendedDeploymentProfile navigation property.|
|[Add intendedDeploymentProfile](../api/windowsautopilotdeviceidentity-post-intendeddeploymentprofile.md)|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|Add intendedDeploymentProfile by posting to the intendedDeploymentProfile collection.|
|[Remove intendedDeploymentProfile](../api/windowsautopilotdeviceidentity-delete-intendeddeploymentprofile.md)|None|Remove an [windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addressableUserName|String|Addressable user name.|
|azureActiveDirectoryDeviceId|String|AAD Device ID|
|deploymentProfileAssignedDateTime|DateTimeOffset|Profile set time of the Windows autopilot device.|
|deploymentProfileAssignmentDetailedStatus|windowsAutopilotProfileAssignmentDetailedStatus|Profile assignment detailed status of the Windows autopilot device. Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.|
|deploymentProfileAssignmentStatus|windowsAutopilotProfileAssignmentStatus|Profile assignment status of the Windows autopilot device. Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.|
|displayName|String|Display Name|
|enrollmentState|enrollmentState|Intune enrollment state of the Windows autopilot device. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|groupTag|String|Group Tag of the Windows autopilot device.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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

