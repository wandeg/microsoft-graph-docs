---
title: "androidDeviceComplianceLocalActionLockDeviceWithPasscode resource type"
description: "Local Action Lock Device with Passcode Configuration"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidDeviceComplianceLocalActionLockDeviceWithPasscode resource type


Namespace: microsoft.graph

Local Action Lock Device with Passcode Configuration


Inherits from [androidDeviceComplianceLocalActionBase](../resources/androiddevicecompliancelocalactionbase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidDeviceComplianceLocalActionLockDeviceWithPasscodes](../api/androiddevicecompliancelocalactionlockdevicewithpasscode-list.md)|[androidDeviceComplianceLocalActionLockDeviceWithPasscode](../resources/androiddevicecompliancelocalactionlockdevicewithpasscode.md) collection|List properties and relationships of the [androidDeviceComplianceLocalActionLockDeviceWithPasscode](../resources/androiddevicecompliancelocalactionlockdevicewithpasscode.md) objects.|
|[Get androidDeviceComplianceLocalActionLockDeviceWithPasscode](../api/androiddevicecompliancelocalactionlockdevicewithpasscode-get.md)|[androidDeviceComplianceLocalActionLockDeviceWithPasscode](../resources/androiddevicecompliancelocalactionlockdevicewithpasscode.md)|Read properties and relationships of the [androidDeviceComplianceLocalActionLockDeviceWithPasscode](../resources/androiddevicecompliancelocalactionlockdevicewithpasscode.md) object.|
|[Create androidDeviceComplianceLocalActionLockDeviceWithPasscode](../api/androiddevicecompliancelocalactionlockdevicewithpasscode-create.md)|[androidDeviceComplianceLocalActionLockDeviceWithPasscode](../resources/androiddevicecompliancelocalactionlockdevicewithpasscode.md)|Create a new [androidDeviceComplianceLocalActionLockDeviceWithPasscode](../resources/androiddevicecompliancelocalactionlockdevicewithpasscode.md) object.|
|[Delete androidDeviceComplianceLocalActionLockDeviceWithPasscode](../api/androiddevicecompliancelocalactionlockdevicewithpasscode-delete.md)|None|Deletes a [androidDeviceComplianceLocalActionLockDeviceWithPasscode](../resources/androiddevicecompliancelocalactionlockdevicewithpasscode.md).|
|[Update androidDeviceComplianceLocalActionLockDeviceWithPasscode](../api/androiddevicecompliancelocalactionlockdevicewithpasscode-update.md)|[androidDeviceComplianceLocalActionLockDeviceWithPasscode](../resources/androiddevicecompliancelocalactionlockdevicewithpasscode.md)|Update the properties of a [androidDeviceComplianceLocalActionLockDeviceWithPasscode](../resources/androiddevicecompliancelocalactionlockdevicewithpasscode.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|gracePeriodInMinutes|Int32|Number of minutes to wait till a local action is enforced. Valid values 0 to 2147483647 Inherited from [androidDeviceComplianceLocalActionBase](../resources/androiddevicecompliancelocalactionbase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|passcode|String|Passcode to reset to Android device. This property is read-only.|
|passcodeSignInFailureCountBeforeWipe|Int32|Number of sign in failures before wiping device, the value can be 4-11. Valid values 4 to 11|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceComplianceLocalActionLockDeviceWithPasscode",
  "baseType": "microsoft.graph.androidDeviceComplianceLocalActionBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceComplianceLocalActionLockDeviceWithPasscode",
  "id": "String (identifier)",
  "gracePeriodInMinutes": 1024,
  "passcode": "String",
  "passcodeSignInFailureCountBeforeWipe": 1024
}
```

