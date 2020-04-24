---
title: "deliveryOptimizationMaxCacheSizeAbsolute resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deliveryOptimizationMaxCacheSizeAbsolute resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [deliveryOptimizationMaxCacheSize](../resources/deliveryoptimizationmaxcachesize.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|maximumCacheSizeInGigabytes|Int64|Specifies the maximum size in GB of Delivery Optimization cache. Valid values 0 to 4294967295
The value 0 (zero) means "unlimited" cache. Delivery Optimization will clear the cache when the device is running low on disk space. Valid values 0 to 4294967295|

## Relationships
None

## JSON representation
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

