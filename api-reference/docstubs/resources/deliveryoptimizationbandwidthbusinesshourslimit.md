---
title: "deliveryOptimizationBandwidthBusinessHoursLimit resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deliveryOptimizationBandwidthBusinessHoursLimit resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bandwidthBeginBusinessHours|Int32|Specifies the beginning of business hours using a 24-hour clock (0-23). Valid values 0 to 23|
|bandwidthEndBusinessHours|Int32|Specifies the end of business hours using a 24-hour clock (0-23). Valid values 0 to 23|
|bandwidthPercentageDuringBusinessHours|Int32|Specifies the percentage of bandwidth to limit during business hours (0-100). Valid values 0 to 100|
|bandwidthPercentageOutsideBusinessHours|Int32|Specifies the percentage of bandwidth to limit outsidse business hours (0-100). Valid values 0 to 100|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```

