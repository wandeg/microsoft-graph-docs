---
title: "mobileAppInstallSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppInstallSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppInstallSummary](../api/mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[Update mobileAppInstallSummary](../api/mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Update the properties of a [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32||
|failedUserCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32||
|installedUserCount|Int32||
|notApplicableDeviceCount|Int32||
|notApplicableUserCount|Int32||
|notInstalledDeviceCount|Int32||
|notInstalledUserCount|Int32||
|pendingInstallDeviceCount|Int32||
|pendingInstallUserCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```

