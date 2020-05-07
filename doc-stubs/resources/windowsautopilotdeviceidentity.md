---
title: "windowsAutopilotDeviceIdentity resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsAutopilotDeviceIdentity resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
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
|[List assignedDevices](../api/windowsautopilotdeploymentprofile-list-assigneddevices.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) collection|Get the windowsAutopilotDeviceIdentities from the assignedDevices navigation property.|
|[Create assignedDevices](../api/windowsautopilotdeploymentprofile-post-assigneddevices.md)|[windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md)|Create a new assignedDevices object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addressableUserName|String|**TODO: Add Description**|
|azureActiveDirectoryDeviceId|String|**TODO: Add Description**|
|deploymentProfileAssignedDateTime|DateTimeOffset|**TODO: Add Description**|
|deploymentProfileAssignmentDetailedStatus|windowsAutopilotProfileAssignmentDetailedStatus|**TODO: Add Description**. Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.|
|deploymentProfileAssignmentStatus|windowsAutopilotProfileAssignmentStatus|**TODO: Add Description**. Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.|
|displayName|String|**TODO: Add Description**|
|enrollmentState|enrollmentState|**TODO: Add Description**. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|groupTag|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastContactedDateTime|DateTimeOffset|**TODO: Add Description**|
|managedDeviceId|String|**TODO: Add Description**|
|manufacturer|String|**TODO: Add Description**|
|model|String|**TODO: Add Description**|
|orderIdentifier|String|**TODO: Add Description**|
|productKey|String|**TODO: Add Description**|
|purchaseOrderIdentifier|String|**TODO: Add Description**|
|resourceName|String|**TODO: Add Description**|
|serialNumber|String|**TODO: Add Description**|
|skuNumber|String|**TODO: Add Description**|
|systemFamily|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deploymentProfile|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|**TODO: Add Description**|
|intendedDeploymentProfile|[windowsAutopilotDeploymentProfile](../resources/windowsautopilotdeploymentprofile.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

