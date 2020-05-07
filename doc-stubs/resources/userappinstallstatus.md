---
title: "userAppInstallStatus resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userAppInstallStatus resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List app](../api/userappinstallstatus-list-app.md)|[mobileApp](../resources/mobileapp.md) collection|Get the mobileApps from the app navigation property.|
|[Add app](../api/userappinstallstatus-post-app.md)|[mobileApp](../resources/mobileapp.md)|Add app by posting to the app collection.|
|[Remove app](../api/userappinstallstatus-delete-app.md)|None|Remove an [mobileApp](../resources/mobileapp.md) object.|
|[List deviceStatuses](../api/userappinstallstatus-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|Get the mobileAppInstallStatus from the deviceStatuses navigation property.|
|[Create deviceStatuses](../api/userappinstallstatus-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Create a new deviceStatuses object.|
|[Delete deviceStatuses](../api/userappinstallstatus-delete-devicestatuses.md)|None|Delete a [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object.|
|[Update deviceStatuses](../api/userappinstallstatus-update-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Update the properties of a deviceStatuses object.|
|[Get mobileAppInstallStatus](../api/mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Read the properties and relationships of a [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object.|
|[List userStatuses](../api/mobileapp-list-userstatuses.md)|[userAppInstallStatus](../resources/userappinstallstatus.md) collection|Get the userAppInstallStatus from the userStatuses navigation property.|
|[Create userStatuses](../api/mobileapp-post-userstatuses.md)|[userAppInstallStatus](../resources/userappinstallstatus.md)|Create a new userStatuses object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|failedDeviceCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|**TODO: Add Description**|
|notInstalledDeviceCount|Int32|**TODO: Add Description**|
|userName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|app|[mobileApp](../resources/mobileapp.md)|**TODO: Add Description**|
|deviceStatuses|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "installedDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "notInstalledDeviceCount": "Integer"
}
```

