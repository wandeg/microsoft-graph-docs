---
title: "networkInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# networkInfo resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bandwidthLowEventRatio|Single|**TODO: Add Description**|
|basicServiceSetIdentifier|String|**TODO: Add Description**|
|connectionType|networkConnectionType|**TODO: Add Description**. Possible values are: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.|
|delayEventRatio|Single|**TODO: Add Description**|
|dnsSuffix|String|**TODO: Add Description**|
|ipAddress|String|**TODO: Add Description**|
|linkSpeed|Int64|**TODO: Add Description**|
|macAddress|String|**TODO: Add Description**|
|port|Int32|**TODO: Add Description**|
|receivedQualityEventRatio|Single|**TODO: Add Description**|
|reflexiveIPAddress|String|**TODO: Add Description**|
|relayIPAddress|String|**TODO: Add Description**|
|relayPort|Int32|**TODO: Add Description**|
|sentQualityEventRatio|Single|**TODO: Add Description**|
|subnet|String|**TODO: Add Description**|
|wifiBand|wifiBand|**TODO: Add Description**. Possible values are: `unknown`, `frequency24GHz`, `frequency50GHz`.|
|wifiBatteryCharge|Int32|**TODO: Add Description**|
|wifiChannel|Int32|**TODO: Add Description**|
|wifiMicrosoftDriver|String|**TODO: Add Description**|
|wifiMicrosoftDriverVersion|String|**TODO: Add Description**|
|wifiRadioType|wifiRadioType|**TODO: Add Description**. Possible values are: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.|
|wifiSignalStrength|Int32|**TODO: Add Description**|
|wifiVendorDriver|String|**TODO: Add Description**|
|wifiVendorDriverVersion|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.networkInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.networkInfo",
  "ipAddress": "String",
  "subnet": "String",
  "linkSpeed": 1024,
  "connectionType": "String",
  "port": 1024,
  "reflexiveIPAddress": "String",
  "relayIPAddress": "String",
  "relayPort": 1024,
  "macAddress": "String",
  "wifiMicrosoftDriver": "String",
  "wifiMicrosoftDriverVersion": "String",
  "wifiVendorDriver": "String",
  "wifiVendorDriverVersion": "String",
  "wifiChannel": 1024,
  "wifiBand": "String",
  "basicServiceSetIdentifier": "String",
  "wifiRadioType": "String",
  "wifiSignalStrength": 1024,
  "wifiBatteryCharge": 1024,
  "dnsSuffix": "String",
  "sentQualityEventRatio": "Single",
  "receivedQualityEventRatio": "Single",
  "delayEventRatio": "Single",
  "bandwidthLowEventRatio": "Single"
}
```

