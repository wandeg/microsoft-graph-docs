---
title: "deviceManagementScriptRunSummary resource type"
description: "Contains properties for the run summary of a device management script."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementScriptRunSummary resource type


Namespace: microsoft.graph

Contains properties for the run summary of a device management script.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|errorDeviceCount|Int32|Error device count.|
|errorUserCount|Int32|Error user count.|
|id|String|Key of the device management script run summary entity. This property is read-only.|
|successDeviceCount|Int32|Success device count.|
|successUserCount|Int32|Success user count.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.deviceManagementScriptRunSummary",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "successUserCount": "Integer",
  "errorUserCount": "Integer"
}
```

