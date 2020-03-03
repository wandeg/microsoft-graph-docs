---
title: "deviceManagementPartner resource type"
description: "Entity which represents a connection to device management partner."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementPartner resource type

Entity which represents a connection to device management partner.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementPartner](../api/devicemanagementpartner-get.md)|[deviceManagementPartner](../resources/deviceManagementPartner.md)|Read properties and relationships of the [deviceManagementPartner](../resources/devicemanagementpartner.md) object.|
|[Delete deviceManagementPartner](../api/devicemanagementpartner-delete.md)|None|Deletes a [deviceManagementPartner](../resources/devicemanagementpartner.md).|
|[Update deviceManagementPartner](../api/devicemanagementpartner-update.md)|[deviceManagementPartner](../resources/deviceManagementPartner.md)|Update the properties of a [deviceManagementPartner](../resources/devicemanagementpartner.md) object.|
|[List deviceManagementPartners](../api/intune-devices-devicemanagement-list-devicemanagementpartners.md)|[deviceManagementPartner](../resources/deviceManagementPartner.md) collection|Get the deviceManagementPartners from the deviceManagementPartners navigation property.|
|[Add deviceManagementPartners](../api/intune-devices-devicemanagement-post-devicemanagementpartners.md)|[deviceManagementPartner](../resources/deviceManagementPartner.md)|Add deviceManagementPartners by posting to the deviceManagementPartners collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Partner display name|
|groupsRequiringPartnerEnrollment|[deviceManagementPartnerAssignment](../resources/deviceManagementPartnerAssignment.md) collection|User groups that specifies whether enrollment is through partner.|
|id|String| Inherited from [entity](../resources/entity.md)|
|isConfigured|Boolean|Whether device management partner is configured or not|
|lastHeartbeatDateTime|DateTimeOffset|Timestamp of last heartbeat after admin enabled option Connect to Device management Partner|
|partnerAppType|Enumeration|Partner App type. Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.|
|partnerState|Enumeration|Partner state of this tenant. Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|singleTenantAppId|String|Partner Single tenant App id|
|whenPartnerDevicesWillBeMarkedAsNonCompliant|DateTimeOffset|DateTime in UTC when PartnerDevices will be marked as NonCompliant. This will become obselete soon.|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|DateTime in UTC when PartnerDevices will be marked as NonCompliant|
|whenPartnerDevicesWillBeRemoved|DateTimeOffset|DateTime in UTC when PartnerDevices will be removed. This will become obselete soon.|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|DateTime in UTC when PartnerDevices will be removed|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "String (timestamp)",
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
    }
  ]
}
```

