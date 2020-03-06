---
title: "windowsInformationProtectionWipeAction resource type"
description: "Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionWipeAction resource type


Namespace: microsoft.graph

Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsInformationProtectionWipeAction](../api/windowsinformationprotectionwipeaction-get.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md)|Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.|
|[Update windowsInformationProtectionWipeAction](../api/windowsinformationprotectionwipeaction-update.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md)|Update the properties of a [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastCheckInDateTime|DateTimeOffset|Last checkin time of the device that was targeted by this wipe action.|
|status|Enumeration|Wipe action status. Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|targetedDeviceMacAddress|String|Targeted device Mac address.|
|targetedDeviceName|String|Targeted device name.|
|targetedDeviceRegistrationId|String|The DeviceRegistrationId being targeted by this wipe action.|
|targetedUserId|String|The UserId being targeted by this wipe action.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "String (identifier)",
  "status": "String",
  "targetedUserId": "String",
  "targetedDeviceRegistrationId": "String",
  "targetedDeviceName": "String",
  "targetedDeviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```

