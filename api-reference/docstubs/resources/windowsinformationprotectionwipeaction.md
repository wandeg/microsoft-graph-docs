---
title: "windowsInformationProtectionWipeAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionWipeAction resource type


Namespace: microsoft.graph




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
|lastCheckInDateTime|DateTimeOffset||
|status|Enumeration| Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|targetedDeviceMacAddress|String||
|targetedDeviceName|String||
|targetedDeviceRegistrationId|String||
|targetedUserId|String||

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

