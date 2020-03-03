---
title: "deliveryOptimizationMaxCacheSizeAbsolute resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deliveryOptimizationMaxCacheSizeAbsolute resource type




Inherits from [deliveryOptimizationMaxCacheSize](../resources/deliveryOptimizationMaxCacheSize.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|maximumCacheSizeInGigabytes|Int64|Specifies the maximum size in GB of Delivery Optimization cache. Valid values 0 to 4294967295
The value 0 (zero) means "unlimited" cache. Delivery Optimization will clear the cache when the device is running low on disk space. Valid values 0 to 4294967295|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute",
  "maximumCacheSizeInGigabytes": 1024
}
```

