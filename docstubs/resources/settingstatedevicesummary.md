---
title: "settingStateDeviceSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# settingStateDeviceSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get settingStateDeviceSummary](../api/settingstatedevicesummary-get.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Read properties and relationships of the [settingStateDeviceSummary](../resources/settingstatedevicesummary.md) object.|
|[Update settingStateDeviceSummary](../api/settingstatedevicesummary-update.md)|[settingStateDeviceSummary](../resources/settingstatedevicesummary.md)|Update the properties of a [settingStateDeviceSummary](../resources/settingstatedevicesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32||
|conflictDeviceCount|Int32||
|errorDeviceCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|instancePath|String||
|nonCompliantDeviceCount|Int32||
|notApplicableDeviceCount|Int32||
|remediatedDeviceCount|Int32||
|settingName|String||
|unknownDeviceCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```

