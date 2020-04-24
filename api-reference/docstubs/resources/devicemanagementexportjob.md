---
title: "deviceManagementExportJob resource type"
description: "Entity representing a job to export a report"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementExportJob resource type


Namespace: microsoft.graph

Entity representing a job to export a report


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementExportJob](../api/devicemanagementexportjob-get.md)|[deviceManagementExportJob](../resources/devicemanagementexportjob.md)|Read the properties and relationships of a [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.|
|[Update deviceManagementExportJob](../api/devicemanagementexportjob-update.md)|[deviceManagementExportJob](../resources/devicemanagementexportjob.md)|Update the properties of a [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset|Time that the exported report expires|
|filter|String|Filters applied on the report|
|format|deviceManagementReportFileFormat|Format of the exported report. Possible values are: `csv`, `pdf`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|reportName|String|Name of the report|
|requestDateTime|DateTimeOffset|Time that the exported report was requested|
|select|String collection|Columns selected from the report|
|snapshotId|String|A snapshot is an identifiable subset of the dataset represented by the ReportName. A sessionId or CachedReportConfiguration id can be used here. If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId. Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.|
|status|deviceManagementReportStatus|Status of the export job. Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|String|Temporary location of the exported report|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExportJob",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "String (identifier)",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "format": "String",
  "snapshotId": "String",
  "status": "String",
  "url": "String",
  "requestDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```

