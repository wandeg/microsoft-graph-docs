---
title: "iosLobAppProvisioningConfiguration resource type"
description: "This topic provides descriptions of the declared methods, properties and relationships exposed by the iOS Lob App Provisioning Configuration resource."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# iosLobAppProvisioningConfiguration resource type

This topic provides descriptions of the declared methods, properties and relationships exposed by the iOS Lob App Provisioning Configuration resource.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get iosLobAppProvisioningConfiguration](../api/intune-apps-ioslobappprovisioningconfiguration-get.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-iosLobAppProvisioningConfiguration.md)|Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md) object.|
|[Delete iosLobAppProvisioningConfiguration](../api/intune-apps-ioslobappprovisioningconfiguration-delete.md)|None|Deletes a [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md).|
|[Update iosLobAppProvisioningConfiguration](../api/intune-apps-ioslobappprovisioningconfiguration-update.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-iosLobAppProvisioningConfiguration.md)|Update the properties of a [iosLobAppProvisioningConfiguration](../resources/ioslobappprovisioningconfiguration.md) object.|
|[assign](../api/intune-apps-ioslobappprovisioningconfiguration-assign.md)|None||
|[hasPayloadLinks](../api/intune-apps-ioslobappprovisioningconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/hasPayloadLinkResultItem.md) collection||
|[List groupAssignments](../api/intune-apps-ioslobappprovisioningconfiguration-list-groupassignments.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileAppProvisioningConfigGroupAssignment.md) collection|Get the mobileAppProvisioningConfigGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/intune-apps-ioslobappprovisioningconfiguration-post-groupassignments.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileAppProvisioningConfigGroupAssignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/intune-apps-ioslobappprovisioningconfiguration-list-assignments.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-iosLobAppProvisioningConfigurationAssignment.md) collection|Get the iosLobAppProvisioningConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/intune-apps-ioslobappprovisioningconfiguration-post-assignments.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-iosLobAppProvisioningConfigurationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/intune-apps-ioslobappprovisioningconfiguration-list-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationDeviceStatus.md) collection|Get the managedDeviceMobileAppConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/intune-apps-ioslobappprovisioningconfiguration-post-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationDeviceStatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/intune-apps-ioslobappprovisioningconfiguration-list-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationUserStatus.md) collection|Get the managedDeviceMobileAppConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/intune-apps-ioslobappprovisioningconfiguration-post-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationUserStatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[List iosLobAppProvisioningConfigurations](../api/intune-apps-deviceappmanagement-list-ioslobappprovisioningconfigurations.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-iosLobAppProvisioningConfiguration.md) collection|Get the iosLobAppProvisioningConfigurations from the iosLobAppProvisioningConfigurations navigation property.|
|[Add iosLobAppProvisioningConfigurations](../api/intune-apps-deviceappmanagement-post-ioslobappprovisioningconfigurations.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-iosLobAppProvisioningConfiguration.md)|Add iosLobAppProvisioningConfigurations by posting to the iosLobAppProvisioningConfigurations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the Device Configuration.|
|displayName|String|Admin provided name of the device configuration.|
|expirationDateTime|DateTimeOffset|Optional profile expiration date and time.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|payload|Binary|Payload. (UTF8 encoded byte array)|
|payloadFileName|String|Payload file name (*.mobileprovision | *.xml).|
|roleScopeTagIds|String collection|List of Scope Tags for this iOS LOB app provisioning configuration entity.|
|version|Int32|Version of the device configuration.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-iosLobAppProvisioningConfigurationAssignment.md) collection|The associated group assignments for IosLobAppProvisioningConfiguration.|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationDeviceStatus.md) collection|The list of device installation states for this mobile app configuration.|
|groupAssignments|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileAppProvisioningConfigGroupAssignment.md) collection|The associated group assignments.|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-managedDeviceMobileAppConfigurationUserStatus.md) collection|The list of user installation states for this mobile app configuration.|

## JSON Representation
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

