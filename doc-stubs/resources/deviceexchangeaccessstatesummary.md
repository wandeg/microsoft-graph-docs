---
title: "deviceExchangeAccessStateSummary resource type"
description: "Device Exchange Access State summary"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceExchangeAccessStateSummary resource type


Namespace: microsoft.graph

Device Exchange Access State summary

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedDeviceCount|Int32|Total count of devices with Exchange Access State: Allowed.|
|blockedDeviceCount|Int32|Total count of devices with Exchange Access State: Blocked.|
|quarantinedDeviceCount|Int32|Total count of devices with Exchange Access State: Quarantined.|
|unavailableDeviceCount|Int32|Total count of devices for which no Exchange Access State could be found.|
|unknownDeviceCount|Int32|Total count of devices with Exchange Access State: Unknown.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": "Integer",
  "blockedDeviceCount": "Integer",
  "quarantinedDeviceCount": "Integer",
  "unknownDeviceCount": "Integer",
  "unavailableDeviceCount": "Integer"
}
```

