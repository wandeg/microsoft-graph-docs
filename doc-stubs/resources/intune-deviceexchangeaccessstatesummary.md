---
title: "deviceExchangeAccessStateSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceExchangeAccessStateSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedDeviceCount|Int32|**TODO: Add Description**|
|blockedDeviceCount|Int32|**TODO: Add Description**|
|quarantinedDeviceCount|Int32|**TODO: Add Description**|
|unavailableDeviceCount|Int32|**TODO: Add Description**|
|unknownDeviceCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": "Integer",
  "blockedDeviceCount": "Integer",
  "quarantinedDeviceCount": "Integer",
  "unknownDeviceCount": "Integer",
  "unavailableDeviceCount": "Integer"
}
```

