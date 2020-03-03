---
title: "deviceInstallState resource type"
description: "Contains properties for the installation state for a device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceInstallState resource type

Contains properties for the installation state for a device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceInstallState](../api/deviceinstallstate-get.md)|[deviceInstallState](../resources/deviceInstallState.md)|Read properties and relationships of the [deviceInstallState](../resources/deviceinstallstate.md) object.|
|[Delete deviceInstallState](../api/deviceinstallstate-delete.md)|None|Deletes a [deviceInstallState](../resources/deviceinstallstate.md).|
|[Update deviceInstallState](../api/deviceinstallstate-update.md)|[deviceInstallState](../resources/deviceInstallState.md)|Update the properties of a [deviceInstallState](../resources/deviceinstallstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceId|String|Device Id.|
|deviceName|String|Device name.|
|errorCode|String|The error code for install failures.|
|id|String| Inherited from [entity](../resources/entity.md)|
|installState|Enumeration|The install state of the eBook. Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.|
|lastSyncDateTime|DateTimeOffset|Last sync date and time.|
|osDescription|String|OS Description.|
|osVersion|String|OS Version.|
|userName|String|Device User Name.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```

