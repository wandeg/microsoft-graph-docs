---
title: "userAppInstallStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userAppInstallStatus resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userAppInstallStatus](../api/userappinstallstatus-get.md)|[userAppInstallStatus](../resources/userappinstallstatus.md)|Read properties and relationships of the [userAppInstallStatus](../resources/userappinstallstatus.md) object.|
|[Update userAppInstallStatus](../api/userappinstallstatus-update.md)|[userAppInstallStatus](../resources/userappinstallstatus.md)|Update the properties of a [userAppInstallStatus](../resources/userappinstallstatus.md) object.|
|[Get mobileApp](../api/mobileapp-get.md)|[mobileApp](../resources/mobileapp.md)|Read properties and relationships of the [mobileApp](../resources/mobileapp.md) object.|
|[List deviceStatuses](../api/userappinstallstatus-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/userappinstallstatus-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/mobileapp-list-userstatuses.md)|[userAppInstallStatus](../resources/userappinstallstatus.md) collection|Get the userAppInstallStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/mobileapp-post-userstatuses.md)|[userAppInstallStatus](../resources/userappinstallstatus.md)|Add userStatuses by posting to the userStatuses collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32||
|notInstalledDeviceCount|Int32||
|userName|String||
|userPrincipalName|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|app|[mobileApp](../resources/mobileapp.md)||
|deviceStatuses|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAppInstallStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "String (identifier)",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```

