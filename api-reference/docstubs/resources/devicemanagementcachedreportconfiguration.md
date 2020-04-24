---
title: "deviceManagementCachedReportConfiguration resource type"
description: "Entity representing the configuration of a cached report"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementCachedReportConfiguration resource type


Namespace: microsoft.graph

Entity representing the configuration of a cached report


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementCachedReportConfiguration](../api/devicemanagementcachedreportconfiguration-get.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Read the properties and relationships of a [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.|
|[Update deviceManagementCachedReportConfiguration](../api/devicemanagementcachedreportconfiguration-update.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Update the properties of a [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset|Time that the cached report expires|
|filter|String|Filters applied on report creation.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastRefreshDateTime|DateTimeOffset|Time that the cached report was last refreshed|
|orderBy|String collection|Ordering of columns in the report|
|reportName|String|Name of the report|
|select|String collection|Columns selected from the report|
|status|deviceManagementReportStatus|Status of the cached report. Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|

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

