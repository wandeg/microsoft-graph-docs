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
|[List windowsInformationProtectionWipeActions](../api/windowsinformationprotectionwipeaction-list.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) collection|List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) objects.|
|[Get windowsInformationProtectionWipeAction](../api/windowsinformationprotectionwipeaction-get.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md)|Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.|
|[Create windowsInformationProtectionWipeAction](../api/windowsinformationprotectionwipeaction-create.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md)|Create a new [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.|
|[Delete windowsInformationProtectionWipeAction](../api/windowsinformationprotectionwipeaction-delete.md)|None|Deletes a [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md).|
|[Update windowsInformationProtectionWipeAction](../api/windowsinformationprotectionwipeaction-update.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md)|Update the properties of a [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.|
|[List windowsInformationProtectionWipeActions](../api/intune-apps-deviceappmanagement-list-windowsinformationprotectionwipeactions.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) collection|Get the windowsInformationProtectionWipeActions from the windowsInformationProtectionWipeActions navigation property.|
|[Add windowsInformationProtectionWipeActions](../api/intune-apps-deviceappmanagement-post-windowsinformationprotectionwipeactions.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md)|Add windowsInformationProtectionWipeActions by posting to the windowsInformationProtectionWipeActions collection.|

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

## JSON Representation
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

