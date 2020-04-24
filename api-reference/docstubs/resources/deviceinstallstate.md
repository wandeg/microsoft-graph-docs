---
title: "deviceInstallState resource type"
description: "Contains properties for the installation state for a device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceInstallState resource type


Namespace: microsoft.graph

Contains properties for the installation state for a device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceInstallState](../api/deviceinstallstate-get.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Read the properties and relationships of a [deviceInstallState](../resources/deviceinstallstate.md) object.|
|[Update deviceInstallState](../api/deviceinstallstate-update.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Update the properties of a [deviceInstallState](../resources/deviceinstallstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceId|String|Device Id.|
|deviceName|String|Device name.|
|errorCode|String|The error code for install failures.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|installState|installState|The install state of the eBook. Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.|
|lastSyncDateTime|DateTimeOffset|Last sync date and time.|
|osDescription|String|OS Description.|
|osVersion|String|OS Version.|
|userName|String|Device User Name.|

## Relationships
None

## JSON representation
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

