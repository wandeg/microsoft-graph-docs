---
title: "eBookInstallSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# eBookInstallSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get eBookInstallSummary](../api/ebookinstallsummary-get.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Read properties and relationships of the [eBookInstallSummary](../resources/ebookinstallsummary.md) object.|
|[Update eBookInstallSummary](../api/ebookinstallsummary-update.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Update the properties of a [eBookInstallSummary](../resources/ebookinstallsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32||
|failedUserCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32||
|installedUserCount|Int32||
|notInstalledDeviceCount|Int32||
|notInstalledUserCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```

