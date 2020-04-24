---
title: "deviceManagementIntentDeviceState resource type"
description: "Entity that represents device state for an intent"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementIntentDeviceState resource type


Namespace: microsoft.graph

Entity that represents device state for an intent


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementIntentDeviceState](../api/devicemanagementintentdevicestate-get.md)|[deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md)|Read the properties and relationships of a [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) object.|
|[Update deviceManagementIntentDeviceState](../api/devicemanagementintentdevicestate-update.md)|[deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md)|Update the properties of a [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceDisplayName|String|Device name that is being reported|
|deviceId|String|Device id that is being reported|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastReportedDateTime|DateTimeOffset|Last modified date time of an intent report|
|state|complianceStatus|Device state for an intent. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userName|String|The user name that is being reported on a device|
|userPrincipalName|String|The user principal name that is being reported on a device|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceDisplayName": "String",
  "lastReportedDateTime": "String (timestamp)",
  "state": "String",
  "deviceId": "String"
}
```

