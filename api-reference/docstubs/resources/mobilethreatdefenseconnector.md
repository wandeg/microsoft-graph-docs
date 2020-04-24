---
title: "mobileThreatDefenseConnector resource type"
description: "Entity which represents a connection to Mobile threat defense partner."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mobileThreatDefenseConnector resource type


Namespace: microsoft.graph

Entity which represents a connection to Mobile threat defense partner.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get mobileThreatDefenseConnector](../api/mobilethreatdefenseconnector-get.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md)|Read the properties and relationships of a [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.|
|[Update mobileThreatDefenseConnector](../api/mobilethreatdefenseconnector-update.md)|[mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md)|Update the properties of a [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowPartnerToCollectIOSApplicationMetadata|Boolean|For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune|
|androidDeviceBlockedOnMissingPartnerData|Boolean|For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant|
|androidEnabled|Boolean|For Android, set whether data from the data sync partner should be used during compliance evaluations|
|androidMobileApplicationManagementEnabled|Boolean|For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations. Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|iosDeviceBlockedOnMissingPartnerData|Boolean|For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant|
|iosEnabled|Boolean|For IOS, get or set whether data from the data sync partner should be used during compliance evaluations|
|iosMobileApplicationManagementEnabled|Boolean|For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations. Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.|
|lastHeartbeatDateTime|DateTimeOffset|DateTime of last Heartbeat recieved from the Data Sync Partner|
|macDeviceBlockedOnMissingPartnerData|Boolean|For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant|
|macEnabled|Boolean|For Mac, get or set whether data from the data sync partner should be used during compliance evaluations|
|partnerState|mobileThreatPartnerTenantState|Data Sync Partner state for this account. Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.|
|partnerUnresponsivenessThresholdInDays|Int32|Get or Set days the per tenant tolerance to unresponsiveness for this partner integration|
|partnerUnsupportedOsVersionBlocked|Boolean|Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner|
|windowsDeviceBlockedOnMissingPartnerData|Boolean|For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant|
|windowsEnabled|Boolean|For Windows, get or set whether data from the data sync partner should be used during compliance evaluations|

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

