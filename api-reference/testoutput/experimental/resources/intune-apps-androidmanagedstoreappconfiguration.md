---
title: "androidManagedStoreAppConfiguration resource type"
description: "Contains properties, inherited properties and actions for Android Enterprise mobile app configurations."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# androidManagedStoreAppConfiguration resource type

Contains properties, inherited properties and actions for Android Enterprise mobile app configurations.


Inherits from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List androidManagedStoreAppConfigurations](../api/intune-apps-androidmanagedstoreappconfiguration-list.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidManagedStoreAppConfiguration.md) collection|List properties and relationships of the [androidManagedStoreAppConfiguration](../resources/androidmanagedstoreappconfiguration.md) objects.|
|[Get androidManagedStoreAppConfiguration](../api/intune-apps-androidmanagedstoreappconfiguration-get.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidManagedStoreAppConfiguration.md)|Read properties and relationships of the [androidManagedStoreAppConfiguration](../resources/androidmanagedstoreappconfiguration.md) object.|
|[Create androidManagedStoreAppConfiguration](../api/intune-apps-androidmanagedstoreappconfiguration-create.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidManagedStoreAppConfiguration.md)|Create a new [androidManagedStoreAppConfiguration](../resources/androidmanagedstoreappconfiguration.md) object.|
|[Delete androidManagedStoreAppConfiguration](../api/intune-apps-androidmanagedstoreappconfiguration-delete.md)|None|Deletes a [androidManagedStoreAppConfiguration](../resources/androidmanagedstoreappconfiguration.md).|
|[Update androidManagedStoreAppConfiguration](../api/intune-apps-androidmanagedstoreappconfiguration-update.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidManagedStoreAppConfiguration.md)|Update the properties of a [androidManagedStoreAppConfiguration](../resources/androidmanagedstoreappconfiguration.md) object.|
|[assign](../api/intune-apps-androidmanagedstoreappconfiguration-assign.md)|None||
|[List assignments](../api/intune-apps-androidmanagedstoreappconfiguration-list-assignments.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-managedDeviceMobileAppConfigurationAssignment.md) collection|Get the managedDeviceMobileAppConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/intune-apps-androidmanagedstoreappconfiguration-post-assignments.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-managedDeviceMobileAppConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/intune-apps-androidmanagedstoreappconfiguration-list-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationDeviceStatus.md) collection|Get the managedDeviceMobileAppConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/intune-apps-androidmanagedstoreappconfiguration-post-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/intune-apps-androidmanagedstoreappconfiguration-list-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationUserStatus.md) collection|Get the managedDeviceMobileAppConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/intune-apps-androidmanagedstoreappconfiguration-post-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get managedDeviceMobileAppConfigurationDeviceSummary](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-managedDeviceMobileAppConfigurationDeviceSummary.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md) object.|
|[Get managedDeviceMobileAppConfigurationUserSummary](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-managedDeviceMobileAppConfigurationUserSummary.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/manageddevicemobileappconfigurationusersummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appSupportsOemConfig|Boolean|Whether or not this AppConfig is an OEMConfig policy.|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-managedDeviceMobileAppConfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-managedDeviceMobileAppConfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-managedDeviceMobileAppConfiguration.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-managedDeviceMobileAppConfiguration.md)|
|packageId|String|Android Enterprise app configuration package id.|
|payloadJson|String|Android Enterprise app configuration JSON payload.|
|permissionActions|[androidPermissionAction](../resources/intune-apps-androidPermissionAction.md) collection|List of Android app permissions and corresponding permission actions.|
|roleScopeTagIds|String collection|List of Scope Tags for this App configuration entity. Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-managedDeviceMobileAppConfiguration.md)|
|targetedMobileApps|String collection|the associated app. Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-managedDeviceMobileAppConfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-managedDeviceMobileAppConfiguration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-managedDeviceMobileAppConfigurationAssignment.md) collection|The list of group assignemenets for app configration. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationDeviceStatus.md) collection|List of ManagedDeviceMobileAppConfigurationDeviceStatus. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-managedDeviceMobileAppConfigurationDeviceSummary.md)|App configuration device status summary. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationUserStatus.md) collection|List of ManagedDeviceMobileAppConfigurationUserStatus. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-managedDeviceMobileAppConfigurationUserSummary.md)|App configuration user status summary. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfiguration",
  "baseType": "microsoft.graph.managedDeviceMobileAppConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "packageId": "String",
  "payloadJson": "String",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "String",
      "action": "String"
    }
  ],
  "appSupportsOemConfig": true
}
```

