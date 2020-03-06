---
title: "deviceManagementScriptRunSummary resource type"
description: "Contains properties for the run summary of a device management script."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementScriptRunSummary resource type


Namespace: microsoft.graph

Contains properties for the run summary of a device management script.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementScriptRunSummary](../api/devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md)|Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object.|
|[Update deviceManagementScriptRunSummary](../api/devicemanagementscriptrunsummary-update.md)|[deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md)|Update the properties of a [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|errorDeviceCount|Int32|Error device count.|
|errorUserCount|Int32|Error user count.|
|id|String| Inherited from [entity](../resources/entity.md)|
|successDeviceCount|Int32|Success device count.|
|successUserCount|Int32|Success user count.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```

