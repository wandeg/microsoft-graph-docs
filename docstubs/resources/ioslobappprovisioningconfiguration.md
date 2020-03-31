---
title: "iosLobAppProvisioningConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosLobAppProvisioningConfiguration resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get iosLobAppProvisioningConfiguration](../api/ioslobappprovisioningconfiguration-get.md)|[iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md)|Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md) object.|
|[Update iosLobAppProvisioningConfiguration](../api/ioslobappprovisioningconfiguration-update.md)|[iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md)|Update the properties of a [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md) object.|
|[assign](../api/ioslobappprovisioningconfiguration-assign.md)|None||
|[hasPayloadLinks](../api/ioslobappprovisioningconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection||
|[List groupAssignments](../api/ioslobappprovisioningconfiguration-list-groupassignments.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md) collection|Get the mobileAppProvisioningConfigGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/ioslobappprovisioningconfiguration-post-groupassignments.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/ioslobappprovisioningconfiguration-list-assignments.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) collection|Get the iosLobAppProvisioningConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/ioslobappprovisioningconfiguration-post-assignments.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/ioslobappprovisioningconfiguration-list-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) collection|Get the managedDeviceMobileAppConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/ioslobappprovisioningconfiguration-post-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/ioslobappprovisioningconfiguration-list-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md) collection|Get the managedDeviceMobileAppConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/ioslobappprovisioningconfiguration-post-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|payload|Binary||
|payloadFileName|String||
|roleScopeTagIds|String collection||
|version|Int32||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) collection||
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) collection||
|groupAssignments|[mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md) collection||
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "String (identifier)",
  "expirationDateTime": "String (timestamp)",
  "payloadFileName": "String",
  "payload": "binary",
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

