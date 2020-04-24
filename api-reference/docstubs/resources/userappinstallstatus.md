---
title: "userAppInstallStatus resource type"
description: "Contains properties for the installation status for a user."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userAppInstallStatus resource type


Namespace: microsoft.graph

Contains properties for the installation status for a user.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userAppInstallStatus](../api/userappinstallstatus-get.md)|[userAppInstallStatus](../resources/userappinstallstatus.md)|Read the properties and relationships of a [userAppInstallStatus](../resources/userappinstallstatus.md) object.|
|[Update userAppInstallStatus](../api/userappinstallstatus-update.md)|[userAppInstallStatus](../resources/userappinstallstatus.md)|Update the properties of a [userAppInstallStatus](../resources/userappinstallstatus.md) object.|
|[List app](../api/userappinstallstatus-list-app.md)|[mobileApp](../resources/mobileapp.md) collection|Get the mobileApps from the app navigation property.|
|[Add app](../api/userappinstallstatus-post-app.md)|[mobileApp](../resources/mobileapp.md)|Add app by posting to the app collection.|
|[Remove app](../api/userappinstallstatus-delete-app.md)|None|Remove an [mobileApp](../resources/mobileapp.md) object.|
|[List deviceStatuses](../api/userappinstallstatus-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|Get the mobileAppInstallStatus from the deviceStatuses navigation property.|
|[Create deviceStatuses](../api/userappinstallstatus-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Create a new deviceStatuses object.|
|[Delete deviceStatuses](../api/userappinstallstatus-delete-devicestatuses.md)|None|Delete a [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object.|
|[Update deviceStatuses](../api/userappinstallstatus-update-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Update the properties of a deviceStatuses object.|
|[Get mobileAppInstallStatus](../api/mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Read the properties and relationships of a [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32|Failed Device Count.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|Installed Device Count.|
|notInstalledDeviceCount|Int32|Not installed device count.|
|userName|String|User name.|
|userPrincipalName|String|User Principal Name.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|app|[mobileApp](../resources/mobileapp.md)|The navigation link to the mobile app.|
|deviceStatuses|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|The install state of the app on devices.|

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

