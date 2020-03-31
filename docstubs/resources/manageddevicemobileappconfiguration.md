---
title: "managedDeviceMobileAppConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedDeviceMobileAppConfiguration resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedDeviceMobileAppConfiguration](../api/manageddevicemobileappconfiguration-get.md)|[managedDeviceMobileAppConfiguration](../resources/manageddevicemobileappconfiguration.md)|Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/manageddevicemobileappconfiguration.md) object.|
|[assign](../api/manageddevicemobileappconfiguration-assign.md)|None||
|[List assignments](../api/manageddevicemobileappconfiguration-list-assignments.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/manageddevicemobileappconfigurationassignment.md) collection|Get the managedDeviceMobileAppConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/manageddevicemobileappconfiguration-post-assignments.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/manageddevicemobileappconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/manageddevicemobileappconfiguration-list-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) collection|Get the managedDeviceMobileAppConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/manageddevicemobileappconfiguration-post-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/manageddevicemobileappconfiguration-list-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md) collection|Get the managedDeviceMobileAppConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/manageddevicemobileappconfiguration-post-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get managedDeviceMobileAppConfigurationDeviceSummary](../api/manageddevicemobileappconfigurationdevicesummary-get.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md) object.|
|[Get managedDeviceMobileAppConfigurationUserSummary](../api/manageddevicemobileappconfigurationusersummary-get.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/manageddevicemobileappconfigurationusersummary.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/manageddevicemobileappconfigurationusersummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|roleScopeTagIds|String collection||
|targetedMobileApps|String collection||
|version|Int32||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/manageddevicemobileappconfigurationassignment.md) collection||
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) collection||
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md)||
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md) collection||
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/manageddevicemobileappconfigurationusersummary.md)||

## JSON representation
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
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```

