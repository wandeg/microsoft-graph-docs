---
title: "importedWindowsAutopilotDeviceIdentity resource type"
description: "Imported windows autopilot devices."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# importedWindowsAutopilotDeviceIdentity resource type


Namespace: microsoft.graph

Imported windows autopilot devices.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List importedWindowsAutopilotDeviceIdentities](../api/importedwindowsautopilotdeviceidentity-list.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) collection|List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) objects.|
|[Get importedWindowsAutopilotDeviceIdentity](../api/importedwindowsautopilotdeviceidentity-get.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md)|Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) object.|
|[Create importedWindowsAutopilotDeviceIdentity](../api/importedwindowsautopilotdeviceidentity-create.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md)|Create a new [importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) object.|
|[Delete importedWindowsAutopilotDeviceIdentity](../api/importedwindowsautopilotdeviceidentity-delete.md)|None|Deletes a [importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md).|
|[Update importedWindowsAutopilotDeviceIdentity](../api/importedwindowsautopilotdeviceidentity-update.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md)|Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) object.|
|[import](../api/importedwindowsautopilotdeviceidentity-import.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) collection||
|[List importedWindowsAutopilotDeviceIdentities](../api/intune-devices-devicemanagement-list-importedwindowsautopilotdeviceidentities.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) collection|Get the importedWindowsAutopilotDeviceIdentities from the importedWindowsAutopilotDeviceIdentities navigation property.|
|[Add importedWindowsAutopilotDeviceIdentities](../api/intune-devices-devicemanagement-post-importedwindowsautopilotdeviceidentities.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md)|Add importedWindowsAutopilotDeviceIdentities by posting to the importedWindowsAutopilotDeviceIdentities collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedUserPrincipalName|String|UPN of the user the device will be assigned|
|groupTag|String|Group Tag of the Windows autopilot device.|
|hardwareIdentifier|Binary|Hardware Blob of the Windows autopilot device.|
|id|String| Inherited from [entity](../resources/entity.md)|
|importId|String|The Import Id of the Windows autopilot device.|
|orderIdentifier|String|Order Id of the Windows autopilot device. - Deprecate|
|productKey|String|Product Key of the Windows autopilot device.|
|serialNumber|String|Serial number of the Windows autopilot device.|
|state|[importedWindowsAutopilotDeviceIdentityState](../resources/importedwindowsautopilotdeviceidentitystate.md)|Current state of the imported device.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "orderIdentifier": "String",
  "groupTag": "String",
  "serialNumber": "String",
  "productKey": "String",
  "importId": "String",
  "hardwareIdentifier": "binary",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
  },
  "assignedUserPrincipalName": "String"
}
```

