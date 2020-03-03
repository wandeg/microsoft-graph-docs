---
title: "yammerDeviceUsageUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# yammerDeviceUsageUserCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List yammerDeviceUsageUserCountses](../api/yammerdeviceusageusercounts-list.md)|[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) collection|List properties and relationships of the [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) objects.|
|[Get yammerDeviceUsageUserCounts](../api/yammerdeviceusageusercounts-get.md)|[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)|Read properties and relationships of the [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) object.|
|[Create yammerDeviceUsageUserCounts](../api/yammerdeviceusageusercounts-create.md)|[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)|Create a new [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) object.|
|[Delete yammerDeviceUsageUserCounts](../api/yammerdeviceusageusercounts-delete.md)|None|Deletes a [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md).|
|[Update yammerDeviceUsageUserCounts](../api/yammerdeviceusageusercounts-update.md)|[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)|Update the properties of a [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidPhone|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|iPad|Int32||
|iPhone|Int32||
|other|Int32||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|web|Int32||
|windowsPhone|Int32||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.yammerDeviceUsageUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "web": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "iPhone": 1024,
  "iPad": 1024,
  "other": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

