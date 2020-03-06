---
title: "windowsInformationProtectionDeviceRegistration resource type"
description: "Represents device registration records for Bring-Your-Own-Device(BYOD) Windows devices."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionDeviceRegistration resource type


Namespace: microsoft.graph

Represents device registration records for Bring-Your-Own-Device(BYOD) Windows devices.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsInformationProtectionDeviceRegistration](../api/windowsinformationprotectiondeviceregistration-get.md)|[windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md)|Read properties and relationships of the [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) object.|
|[Update windowsInformationProtectionDeviceRegistration](../api/windowsinformationprotectiondeviceregistration-update.md)|[windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md)|Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) object.|
|[wipe](../api/windowsinformationprotectiondeviceregistration-wipe.md)|None||
|[List windowsInformationProtectionDeviceRegistrations](../api/user-list-windowsinformationprotectiondeviceregistrations.md)|[windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) collection|Get the windowsInformationProtectionDeviceRegistrations from the windowsInformationProtectionDeviceRegistrations navigation property.|
|[Create windowsInformationProtectionDeviceRegistrations](../api/user-post-windowsinformationprotectiondeviceregistrations.md)|[windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md)|Create windowsInformationProtectionDeviceRegistrations by posting to the windowsInformationProtectionDeviceRegistrations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceMacAddress|String|Device Mac address.|
|deviceName|String|Device name.|
|deviceRegistrationId|String|Device identifier for this device registration record.|
|deviceType|String|Device type, for example, Windows laptop VS Windows phone.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastCheckInDateTime|DateTimeOffset|Last checkin time of the device.|
|userId|String|UserId associated with this device registration record.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "String (identifier)",
  "userId": "String",
  "deviceRegistrationId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "deviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```

