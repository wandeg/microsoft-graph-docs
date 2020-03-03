---
title: "userAppInstallStatus resource type"
description: "Contains properties for the installation status for a user."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userAppInstallStatus resource type


Namespace: microsoft.graph

Contains properties for the installation status for a user.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List userAppInstallStatuses](../api/intune-apps-userappinstallstatus-list.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection|List properties and relationships of the [userAppInstallStatus](../resources/userappinstallstatus.md) objects.|
|[Get userAppInstallStatus](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.|
|[Create userAppInstallStatus](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.|
|[Delete userAppInstallStatus](../api/intune-apps-userappinstallstatus-delete.md)|None|Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).|
|[Update userAppInstallStatus](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.|
|[Get mobileApp](../api/intune-apps-mobileapp-get.md)|[mobileApp](../resources/intune-apps-mobileapp.md)|Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.|
|[List deviceStatuses](../api/intune-apps-userappinstallstatus-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection|Get the mobileAppInstallStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/intune-apps-userappinstallstatus-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32|Failed Device Count.|
|id|String| Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|Installed Device Count.|
|notInstalledDeviceCount|Int32|Not installed device count.|
|userName|String|User name.|
|userPrincipalName|String|User Principal Name.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|app|[mobileApp](../resources/intune-apps-mobileapp.md)|The navigation link to the mobile app.|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection|The install state of the app on devices.|

## JSON Representation
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

