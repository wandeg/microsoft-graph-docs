---
title: "mobileAppInstallSummary resource type"
description: "Contains properties for the installation summary of a mobile app."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileAppInstallSummary resource type


Namespace: microsoft.graph

Contains properties for the installation summary of a mobile app.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileAppInstallSummary](../api/mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Read properties and relationships of the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|
|[Update mobileAppInstallSummary](../api/mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Update the properties of a [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32|Number of Devices that have failed to install this app.|
|failedUserCount|Int32|Number of Users that have 1 or more device that failed to install this app.|
|id|String| Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|Number of Devices that have successfully installed this app.|
|installedUserCount|Int32|Number of Users whose devices have all succeeded to install this app.|
|notApplicableDeviceCount|Int32|Number of Devices that are not applicable for this app.|
|notApplicableUserCount|Int32|Number of Users whose devices were all not applicable for this app.|
|notInstalledDeviceCount|Int32|Number of Devices that does not have this app installed.|
|notInstalledUserCount|Int32|Number of Users that have 1 or more devices that did not install this app.|
|pendingInstallDeviceCount|Int32|Number of Devices that have been notified to install this app.|
|pendingInstallUserCount|Int32|Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.|

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

