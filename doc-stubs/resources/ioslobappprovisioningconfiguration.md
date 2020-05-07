---
title: "iosLobAppProvisioningConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# iosLobAppProvisioningConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[assign](../api/ioslobappprovisioningconfiguration-assign.md)|None|**TODO: Add Description**|
|[hasPayloadLinks](../api/ioslobappprovisioningconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/haspayloadlinkresultitem.md) collection|**TODO: Add Description**|
|[List groupAssignments](../api/ioslobappprovisioningconfiguration-list-groupassignments.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md) collection|Get the mobileAppProvisioningConfigGroupAssignments from the groupAssignments navigation property.|
|[Create groupAssignments](../api/ioslobappprovisioningconfiguration-post-groupassignments.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md)|Create a new groupAssignments object.|
|[Delete groupAssignments](../api/ioslobappprovisioningconfiguration-delete-groupassignments.md)|None|Delete a [mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md) object.|
|[Update groupAssignments](../api/ioslobappprovisioningconfiguration-update-groupassignments.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md)|Update the properties of a groupAssignments object.|
|[Get mobileAppProvisioningConfigGroupAssignment](../api/mobileappprovisioningconfiggroupassignment-get.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md)|Read the properties and relationships of a [mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md) object.|
|[List assignments](../api/ioslobappprovisioningconfiguration-list-assignments.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) collection|Get the iosLobAppProvisioningConfigurationAssignments from the assignments navigation property.|
|[Create assignments](../api/ioslobappprovisioningconfiguration-post-assignments.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/ioslobappprovisioningconfiguration-delete-assignments.md)|None|Delete an [iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) object.|
|[Update assignments](../api/ioslobappprovisioningconfiguration-update-assignments.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md)|Update the properties of an assignments object.|
|[Get iosLobAppProvisioningConfigurationAssignment](../api/ioslobappprovisioningconfigurationassignment-get.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md)|Read the properties and relationships of an [iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) object.|
|[List deviceStatuses](../api/ioslobappprovisioningconfiguration-list-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) collection|Get the managedDeviceMobileAppConfigurationDeviceStatus from the deviceStatuses navigation property.|
|[Create deviceStatuses](../api/ioslobappprovisioningconfiguration-post-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md)|Create a new deviceStatuses object.|
|[Delete deviceStatuses](../api/ioslobappprovisioningconfiguration-delete-devicestatuses.md)|None|Delete a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) object.|
|[Update deviceStatuses](../api/ioslobappprovisioningconfiguration-update-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md)|Update the properties of a deviceStatuses object.|
|[Get managedDeviceMobileAppConfigurationDeviceStatus](../api/manageddevicemobileappconfigurationdevicestatus-get.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md)|Read the properties and relationships of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) object.|
|[List userStatuses](../api/ioslobappprovisioningconfiguration-list-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md) collection|Get the managedDeviceMobileAppConfigurationUserStatus from the userStatuses navigation property.|
|[Create userStatuses](../api/ioslobappprovisioningconfiguration-post-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md)|Create a new userStatuses object.|
|[Delete userStatuses](../api/ioslobappprovisioningconfiguration-delete-userstatuses.md)|None|Delete a [managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md) object.|
|[Update userStatuses](../api/ioslobappprovisioningconfiguration-update-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md)|Update the properties of a userStatuses object.|
|[Get managedDeviceMobileAppConfigurationUserStatus](../api/manageddevicemobileappconfigurationuserstatus-get.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md)|Read the properties and relationships of a [managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|payload|Binary|**TODO: Add Description**|
|payloadFileName|String|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|version|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) collection|**TODO: Add Description**|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) collection|**TODO: Add Description**|
|groupAssignments|[mobileAppProvisioningConfigGroupAssignment](../resources/mobileappprovisioningconfiggroupassignment.md) collection|**TODO: Add Description**|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "payload": "Binary",
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": "Integer"
}
```

