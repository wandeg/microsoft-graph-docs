---
title: "networkInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph.callRecords
---


# networkInfo resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|bandwidthLowEventRatio|Single||
|basicServiceSetIdentifier|String||
|connectionType|Enumeration|. Possible values are: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.|
|delayEventRatio|Single||
|dnsSuffix|String||
|ipAddress|String||
|linkSpeed|Int64||
|macAddress|String||
|port|Int32||
|receivedQualityEventRatio|Single||
|reflexiveIPAddress|String||
|relayIPAddress|String||
|relayPort|Int32||
|sentQualityEventRatio|Single||
|subnet|String||
|wifiBand|Enumeration|. Possible values are: `unknown`, `frequency24GHz`, `frequency50GHz`.|
|wifiBatteryCharge|Int32||
|wifiChannel|Int32||
|wifiMicrosoftDriver|String||
|wifiMicrosoftDriverVersion|String||
|wifiRadioType|Enumeration|. Possible values are: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.|
|wifiSignalStrength|Int32||
|wifiVendorDriver|String||
|wifiVendorDriverVersion|String||

## Relationships
None

## JSON Representation
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

