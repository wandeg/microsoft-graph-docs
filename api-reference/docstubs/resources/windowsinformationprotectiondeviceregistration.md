---
title: "windowsInformationProtectionDeviceRegistration resource type"
description: "Represents device registration records for Bring-Your-Own-Device(BYOD) Windows devices."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsInformationProtectionDeviceRegistration resource type


Namespace: microsoft.graph

Represents device registration records for Bring-Your-Own-Device(BYOD) Windows devices.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsInformationProtectionDeviceRegistration](../api/windowsinformationprotectiondeviceregistration-get.md)|[windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md)|Read the properties and relationships of a [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) object.|
|[Update windowsInformationProtectionDeviceRegistration](../api/windowsinformationprotectiondeviceregistration-update.md)|[windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md)|Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) object.|
|[wipe](../api/windowsinformationprotectiondeviceregistration-wipe.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceMacAddress|String|Device Mac address.|
|deviceName|String|Device name.|
|deviceRegistrationId|String|Device identifier for this device registration record.|
|deviceType|String|Device type, for example, Windows laptop VS Windows phone.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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

