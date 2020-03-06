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
|[Get deviceManagementCachedReportConfiguration](../api/devicemanagementcachedreportconfiguration-get.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Read properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.|
|[Update deviceManagementCachedReportConfiguration](../api/devicemanagementcachedreportconfiguration-update.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Update the properties of a [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.|
|[List cachedReportConfigurations](../api/devicemanagementreports-list-cachedreportconfigurations.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) collection|Get the deviceManagementCachedReportConfigurations from the cachedReportConfigurations navigation property.|
|[Add cachedReportConfigurations](../api/devicemanagementreports-post-cachedreportconfigurations.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Add cachedReportConfigurations by posting to the cachedReportConfigurations collection.|

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

## JSON representation
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

