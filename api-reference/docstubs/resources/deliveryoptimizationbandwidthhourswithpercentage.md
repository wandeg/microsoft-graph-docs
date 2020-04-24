---
title: "deliveryOptimizationBandwidthHoursWithPercentage resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deliveryOptimizationBandwidthHoursWithPercentage resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [deliveryOptimizationBandwidth](../resources/deliveryoptimizationbandwidth.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bandwidthBackgroundPercentageHours|[deliveryOptimizationBandwidthBusinessHoursLimit](../resources/deliveryoptimizationbandwidthbusinesshourslimit.md)|Background download percentage hours.|
|bandwidthForegroundPercentageHours|[deliveryOptimizationBandwidthBusinessHoursLimit](../resources/deliveryoptimizationbandwidthbusinesshourslimit.md)|Foreground download percentage hours.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage",
  "bandwidthBackgroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  },
  "bandwidthForegroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
  }
}
```

