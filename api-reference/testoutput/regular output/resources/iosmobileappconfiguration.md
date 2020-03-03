---
title: "iosMobileAppConfiguration resource type"
description: "Contains properties, inherited properties and actions for iOS mobile app configurations."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# iosMobileAppConfiguration resource type

Contains properties, inherited properties and actions for iOS mobile app configurations.


Inherits from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosMobileAppConfigurations](../api/iosmobileappconfiguration-list.md)|[iosMobileAppConfiguration](../resources/iosMobileAppConfiguration.md) collection|List properties and relationships of the [iosMobileAppConfiguration](../resources/iosmobileappconfiguration.md) objects.|
|[Get iosMobileAppConfiguration](../api/iosmobileappconfiguration-get.md)|[iosMobileAppConfiguration](../resources/iosMobileAppConfiguration.md)|Read properties and relationships of the [iosMobileAppConfiguration](../resources/iosmobileappconfiguration.md) object.|
|[Create iosMobileAppConfiguration](../api/iosmobileappconfiguration-create.md)|[iosMobileAppConfiguration](../resources/iosMobileAppConfiguration.md)|Create a new [iosMobileAppConfiguration](../resources/iosmobileappconfiguration.md) object.|
|[Delete iosMobileAppConfiguration](../api/iosmobileappconfiguration-delete.md)|None|Deletes a [iosMobileAppConfiguration](../resources/iosmobileappconfiguration.md).|
|[Update iosMobileAppConfiguration](../api/iosmobileappconfiguration-update.md)|[iosMobileAppConfiguration](../resources/iosMobileAppConfiguration.md)|Update the properties of a [iosMobileAppConfiguration](../resources/iosmobileappconfiguration.md) object.|
|[assign](../api/iosmobileappconfiguration-assign.md)|None||
|[List assignments](../api/iosmobileappconfiguration-list-assignments.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/managedDeviceMobileAppConfigurationAssignment.md) collection|Get the managedDeviceMobileAppConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/iosmobileappconfiguration-post-assignments.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/managedDeviceMobileAppConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/iosmobileappconfiguration-list-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/managedDeviceMobileAppConfigurationDeviceStatus.md) collection|Get the managedDeviceMobileAppConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/iosmobileappconfiguration-post-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/managedDeviceMobileAppConfigurationDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/iosmobileappconfiguration-list-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/managedDeviceMobileAppConfigurationUserStatus.md) collection|Get the managedDeviceMobileAppConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/iosmobileappconfiguration-post-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/managedDeviceMobileAppConfigurationUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get managedDeviceMobileAppConfigurationDeviceSummary](../api/manageddevicemobileappconfigurationdevicesummary-get.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/managedDeviceMobileAppConfigurationDeviceSummary.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md) object.|
|[Get managedDeviceMobileAppConfigurationUserSummary](../api/manageddevicemobileappconfigurationusersummary-get.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/managedDeviceMobileAppConfigurationUserSummary.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/manageddevicemobileappconfigurationusersummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|encodedSettingXml|Binary|mdm app configuration Base64 binary.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|settings|[appConfigurationSettingItem](../resources/appConfigurationSettingItem.md) collection|app configuration setting items.|
|targetedMobileApps|String collection|the associated app. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/managedDeviceMobileAppConfigurationAssignment.md) collection|The list of group assignemenets for app configration. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/managedDeviceMobileAppConfigurationDeviceStatus.md) collection|List of ManagedDeviceMobileAppConfigurationDeviceStatus. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/managedDeviceMobileAppConfigurationDeviceSummary.md)|App configuration device status summary. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/managedDeviceMobileAppConfigurationUserStatus.md) collection|List of ManagedDeviceMobileAppConfigurationUserStatus. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/managedDeviceMobileAppConfigurationUserSummary.md)|App configuration user status summary. Inherited from [managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosMobileAppConfiguration",
  "baseType": "microsoft.graph.managedDeviceMobileAppConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "encodedSettingXml": "binary",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "String",
      "appConfigKeyType": "String",
      "appConfigKeyValue": "String"
    }
  ]
}
```

