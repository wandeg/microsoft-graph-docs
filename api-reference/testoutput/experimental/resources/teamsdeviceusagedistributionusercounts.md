---
title: "teamsDeviceUsageDistributionUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsDeviceUsageDistributionUserCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List teamsDeviceUsageDistributionUserCountses](../api/teamsdeviceusagedistributionusercounts-list.md)|[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) collection|List properties and relationships of the [teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) objects.|
|[Get teamsDeviceUsageDistributionUserCounts](../api/teamsdeviceusagedistributionusercounts-get.md)|[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)|Read properties and relationships of the [teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) object.|
|[Create teamsDeviceUsageDistributionUserCounts](../api/teamsdeviceusagedistributionusercounts-create.md)|[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)|Create a new [teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) object.|
|[Delete teamsDeviceUsageDistributionUserCounts](../api/teamsdeviceusagedistributionusercounts-delete.md)|None|Deletes a [teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md).|
|[Update teamsDeviceUsageDistributionUserCounts](../api/teamsdeviceusagedistributionusercounts-update.md)|[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)|Update the properties of a [teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidPhone|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|ios|Int64||
|mac|Int64||
|reportPeriod|String||
|reportRefreshDate|Date||
|web|Int64||
|windows|Int64||
|windowsPhone|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsDeviceUsageDistributionUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "web": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "ios": 1024,
  "mac": 1024,
  "windows": 1024,
  "reportPeriod": "String"
}
```

