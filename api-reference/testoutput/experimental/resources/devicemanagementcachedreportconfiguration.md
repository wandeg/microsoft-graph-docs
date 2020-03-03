---
title: "deviceManagementCachedReportConfiguration resource type"
description: "Entity representing the configuration of a cached report"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementCachedReportConfiguration resource type


Namespace: microsoft.graph

Entity representing the configuration of a cached report


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementCachedReportConfigurations](../api/devicemanagementcachedreportconfiguration-list.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) collection|List properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) objects.|
|[Get deviceManagementCachedReportConfiguration](../api/devicemanagementcachedreportconfiguration-get.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Read properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.|
|[Create deviceManagementCachedReportConfiguration](../api/devicemanagementcachedreportconfiguration-create.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Create a new [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.|
|[Delete deviceManagementCachedReportConfiguration](../api/devicemanagementcachedreportconfiguration-delete.md)|None|Deletes a [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md).|
|[Update deviceManagementCachedReportConfiguration](../api/devicemanagementcachedreportconfiguration-update.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Update the properties of a [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset|Time that the cached report expires|
|filter|String|Filters applied on report creation.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastRefreshDateTime|DateTimeOffset|Time that the cached report was last refreshed|
|orderBy|String collection|Ordering of columns in the report|
|reportName|String|Name of the report|
|select|String collection|Columns selected from the report|
|status|Enumeration|Status of the cached report. Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCachedReportConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "String (identifier)",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "status": "String",
  "lastRefreshDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```

