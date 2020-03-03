---
title: "androidDeviceComplianceLocalActionLockDevice resource type"
description: "Local Action Lock Device Only Configuration"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidDeviceComplianceLocalActionLockDevice resource type


Namespace: microsoft.graph

Local Action Lock Device Only Configuration


Inherits from [androidDeviceComplianceLocalActionBase](../resources/androiddevicecompliancelocalactionbase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidDeviceComplianceLocalActionLockDevices](../api/androiddevicecompliancelocalactionlockdevice-list.md)|[androidDeviceComplianceLocalActionLockDevice](../resources/androiddevicecompliancelocalactionlockdevice.md) collection|List properties and relationships of the [androidDeviceComplianceLocalActionLockDevice](../resources/androiddevicecompliancelocalactionlockdevice.md) objects.|
|[Get androidDeviceComplianceLocalActionLockDevice](../api/androiddevicecompliancelocalactionlockdevice-get.md)|[androidDeviceComplianceLocalActionLockDevice](../resources/androiddevicecompliancelocalactionlockdevice.md)|Read properties and relationships of the [androidDeviceComplianceLocalActionLockDevice](../resources/androiddevicecompliancelocalactionlockdevice.md) object.|
|[Create androidDeviceComplianceLocalActionLockDevice](../api/androiddevicecompliancelocalactionlockdevice-create.md)|[androidDeviceComplianceLocalActionLockDevice](../resources/androiddevicecompliancelocalactionlockdevice.md)|Create a new [androidDeviceComplianceLocalActionLockDevice](../resources/androiddevicecompliancelocalactionlockdevice.md) object.|
|[Delete androidDeviceComplianceLocalActionLockDevice](../api/androiddevicecompliancelocalactionlockdevice-delete.md)|None|Deletes a [androidDeviceComplianceLocalActionLockDevice](../resources/androiddevicecompliancelocalactionlockdevice.md).|
|[Update androidDeviceComplianceLocalActionLockDevice](../api/androiddevicecompliancelocalactionlockdevice-update.md)|[androidDeviceComplianceLocalActionLockDevice](../resources/androiddevicecompliancelocalactionlockdevice.md)|Update the properties of a [androidDeviceComplianceLocalActionLockDevice](../resources/androiddevicecompliancelocalactionlockdevice.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|gracePeriodInMinutes|Int32|Number of minutes to wait till a local action is enforced. Valid values 0 to 2147483647 Inherited from [androidDeviceComplianceLocalActionBase](../resources/androiddevicecompliancelocalactionbase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceComplianceLocalActionLockDevice",
  "baseType": "microsoft.graph.androidDeviceComplianceLocalActionBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceComplianceLocalActionLockDevice",
  "id": "String (identifier)",
  "gracePeriodInMinutes": 1024
}
```

