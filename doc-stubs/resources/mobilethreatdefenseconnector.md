---
title: "mobileThreatDefenseConnector resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileThreatDefenseConnector resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowPartnerToCollectIOSApplicationMetadata|Boolean|**TODO: Add Description**|
|androidDeviceBlockedOnMissingPartnerData|Boolean|**TODO: Add Description**|
|androidEnabled|Boolean|**TODO: Add Description**|
|androidMobileApplicationManagementEnabled|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|iosDeviceBlockedOnMissingPartnerData|Boolean|**TODO: Add Description**|
|iosEnabled|Boolean|**TODO: Add Description**|
|iosMobileApplicationManagementEnabled|Boolean|**TODO: Add Description**|
|lastHeartbeatDateTime|DateTimeOffset|**TODO: Add Description**|
|macDeviceBlockedOnMissingPartnerData|Boolean|**TODO: Add Description**|
|macEnabled|Boolean|**TODO: Add Description**|
|partnerState|mobileThreatPartnerTenantState|**TODO: Add Description**. Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.|
|partnerUnresponsivenessThresholdInDays|Int32|**TODO: Add Description**|
|partnerUnsupportedOsVersionBlocked|Boolean|**TODO: Add Description**|
|windowsDeviceBlockedOnMissingPartnerData|Boolean|**TODO: Add Description**|
|windowsEnabled|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileThreatDefenseConnector",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "androidMobileApplicationManagementEnabled": "Boolean",
  "iosMobileApplicationManagementEnabled": "Boolean",
  "androidEnabled": "Boolean",
  "iosEnabled": "Boolean",
  "windowsEnabled": "Boolean",
  "macEnabled": "Boolean",
  "androidDeviceBlockedOnMissingPartnerData": "Boolean",
  "iosDeviceBlockedOnMissingPartnerData": "Boolean",
  "windowsDeviceBlockedOnMissingPartnerData": "Boolean",
  "macDeviceBlockedOnMissingPartnerData": "Boolean",
  "partnerUnsupportedOsVersionBlocked": "Boolean",
  "partnerUnresponsivenessThresholdInDays": "Integer",
  "allowPartnerToCollectIOSApplicationMetadata": "Boolean"
}
```

