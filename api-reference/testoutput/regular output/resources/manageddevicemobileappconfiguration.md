---
title: "managedDeviceMobileAppConfiguration resource type"
description: "An abstract class for Mobile app configuration for enrolled devices."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedDeviceMobileAppConfiguration resource type

An abstract class for Mobile app configuration for enrolled devices.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedDeviceMobileAppConfiguration](../api/manageddevicemobileappconfiguration-get.md)|[managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/manageddevicemobileappconfiguration.md) object.|
|[assign](../api/manageddevicemobileappconfiguration-assign.md)|None||
|[List assignments](../api/manageddevicemobileappconfiguration-list-assignments.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/managedDeviceMobileAppConfigurationAssignment.md) collection|Get the managedDeviceMobileAppConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/manageddevicemobileappconfiguration-post-assignments.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/managedDeviceMobileAppConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/manageddevicemobileappconfiguration-list-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/managedDeviceMobileAppConfigurationDeviceStatus.md) collection|Get the managedDeviceMobileAppConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/manageddevicemobileappconfiguration-post-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/managedDeviceMobileAppConfigurationDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/manageddevicemobileappconfiguration-list-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/managedDeviceMobileAppConfigurationUserStatus.md) collection|Get the managedDeviceMobileAppConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/manageddevicemobileappconfiguration-post-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/managedDeviceMobileAppConfigurationUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get managedDeviceMobileAppConfigurationDeviceSummary](../api/manageddevicemobileappconfigurationdevicesummary-get.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/managedDeviceMobileAppConfigurationDeviceSummary.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md) object.|
|[Get managedDeviceMobileAppConfigurationUserSummary](../api/manageddevicemobileappconfigurationusersummary-get.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/managedDeviceMobileAppConfigurationUserSummary.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/manageddevicemobileappconfigurationusersummary.md) object.|
|[List mobileAppConfigurations](../api/deviceappmanagement-list-mobileappconfigurations.md)|[managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md) collection|Get the managedDeviceMobileAppConfigurations from the mobileAppConfigurations navigation property.|
|[Add mobileAppConfigurations](../api/deviceappmanagement-post-mobileappconfigurations.md)|[managedDeviceMobileAppConfiguration](../resources/managedDeviceMobileAppConfiguration.md)|Add mobileAppConfigurations by posting to the mobileAppConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the Device Configuration.|
|displayName|String|Admin provided name of the device configuration.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|targetedMobileApps|String collection|the associated app.|
|version|Int32|Version of the device configuration.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/managedDeviceMobileAppConfigurationAssignment.md) collection|The list of group assignemenets for app configration.|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/managedDeviceMobileAppConfigurationDeviceStatus.md) collection|List of ManagedDeviceMobileAppConfigurationDeviceStatus.|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/managedDeviceMobileAppConfigurationDeviceSummary.md)|App configuration device status summary.|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/managedDeviceMobileAppConfigurationUserStatus.md) collection|List of ManagedDeviceMobileAppConfigurationUserStatus.|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/managedDeviceMobileAppConfigurationUserSummary.md)|App configuration user status summary.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```

