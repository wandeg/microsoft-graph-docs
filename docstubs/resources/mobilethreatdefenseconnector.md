---
title: "mobileThreatDefenseConnector resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mobileThreatDefenseConnector resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileThreatDefenseConnector](../api/mobilethreatdefenseconnector-get.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md)|Read properties and relationships of the [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.|
|[Update mobileThreatDefenseConnector](../api/mobilethreatdefenseconnector-update.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md)|Update the properties of a [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowPartnerToCollectIOSApplicationMetadata|Boolean||
|androidDeviceBlockedOnMissingPartnerData|Boolean||
|androidEnabled|Boolean||
|androidMobileApplicationManagementEnabled|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|iosDeviceBlockedOnMissingPartnerData|Boolean||
|iosEnabled|Boolean||
|iosMobileApplicationManagementEnabled|Boolean||
|lastHeartbeatDateTime|DateTimeOffset||
|macDeviceBlockedOnMissingPartnerData|Boolean||
|macEnabled|Boolean||
|partnerState|Enumeration| Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.|
|partnerUnresponsivenessThresholdInDays|Int32||
|partnerUnsupportedOsVersionBlocked|Boolean||
|windowsDeviceBlockedOnMissingPartnerData|Boolean||
|windowsEnabled|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 1024,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```

