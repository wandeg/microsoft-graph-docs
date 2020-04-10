---
title: "softwareUpdateStatusSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# softwareUpdateStatusSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get softwareUpdateStatusSummary](../api/softwareupdatestatussummary-get.md)|[softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md)|Read properties and relationships of the [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object.|
|[Update softwareUpdateStatusSummary](../api/softwareupdatestatussummary-update.md)|[softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md)|Update the properties of a [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32||
|compliantUserCount|Int32||
|conflictDeviceCount|Int32||
|conflictUserCount|Int32||
|displayName|String||
|errorDeviceCount|Int32||
|errorUserCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|nonCompliantDeviceCount|Int32||
|nonCompliantUserCount|Int32||
|notApplicableDeviceCount|Int32||
|notApplicableUserCount|Int32||
|remediatedDeviceCount|Int32||
|remediatedUserCount|Int32||
|unknownDeviceCount|Int32||
|unknownUserCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```

