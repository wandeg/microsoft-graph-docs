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


Inherits from [deliveryOptimizationBandwidth](../resources/deliveryoptimizationbandwidth.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bandwidthBackgroundPercentageHours|[deliveryOptimizationBandwidthBusinessHoursLimit](../resources/deliveryoptimizationbandwidthbusinesshourslimit.md)|**TODO: Add Description**|
|bandwidthForegroundPercentageHours|[deliveryOptimizationBandwidthBusinessHoursLimit](../resources/deliveryoptimizationbandwidthbusinesshourslimit.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage",
  "bandwidthBackgroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
  },
  "bandwidthForegroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
  }
}
```

