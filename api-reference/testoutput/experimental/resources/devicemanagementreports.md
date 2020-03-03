---
title: "deviceManagementReports resource type"
description: "Singleton entity that acts as a container for all reports functionality."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementReports resource type

Singleton entity that acts as a container for all reports functionality.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementReportses](../api/devicemanagementreports-list.md)|[deviceManagementReports](../resources/deviceManagementReports.md) collection|List properties and relationships of the [deviceManagementReports](../resources/devicemanagementreports.md) objects.|
|[Get deviceManagementReports](../api/devicemanagementreports-get.md)|[deviceManagementReports](../resources/deviceManagementReports.md)|Read properties and relationships of the [deviceManagementReports](../resources/devicemanagementreports.md) object.|
|[Create deviceManagementReports](../api/devicemanagementreports-create.md)|[deviceManagementReports](../resources/deviceManagementReports.md)|Create a new [deviceManagementReports](../resources/devicemanagementreports.md) object.|
|[Delete deviceManagementReports](../api/devicemanagementreports-delete.md)|None|Deletes a [deviceManagementReports](../resources/devicemanagementreports.md).|
|[Update deviceManagementReports](../api/devicemanagementreports-update.md)|[deviceManagementReports](../resources/deviceManagementReports.md)|Update the properties of a [deviceManagementReports](../resources/devicemanagementreports.md) object.|
|[getDeviceNonComplianceReport](../api/devicemanagementreports-getdevicenoncompliancereport.md)|Stream||
|[getPolicyNonComplianceReport](../api/devicemanagementreports-getpolicynoncompliancereport.md)|Stream||
|[getPolicyNonComplianceMetadata](../api/devicemanagementreports-getpolicynoncompliancemetadata.md)|Stream||
|[getHistoricalReport](../api/devicemanagementreports-gethistoricalreport.md)|Stream||
|[getCachedReport](../api/devicemanagementreports-getcachedreport.md)|Stream||
|[List cachedReportConfigurations](../api/devicemanagementreports-list-cachedreportconfigurations.md)|[deviceManagementCachedReportConfiguration](../resources/deviceManagementCachedReportConfiguration.md) collection|Get the deviceManagementCachedReportConfigurations from the cachedReportConfigurations navigation property.|
|[Add cachedReportConfigurations](../api/devicemanagementreports-post-cachedreportconfigurations.md)|[deviceManagementCachedReportConfiguration](../resources/deviceManagementCachedReportConfiguration.md)|Add cachedReportConfigurations by posting to the cachedReportConfigurations collection.|
|[List exportJobs](../api/devicemanagementreports-list-exportjobs.md)|[deviceManagementExportJob](../resources/deviceManagementExportJob.md) collection|Get the deviceManagementExportJobs from the exportJobs navigation property.|
|[Add exportJobs](../api/devicemanagementreports-post-exportjobs.md)|[deviceManagementExportJob](../resources/deviceManagementExportJob.md)|Add exportJobs by posting to the exportJobs collection.|
|[List reportSchedules](../api/devicemanagementreports-list-reportschedules.md)|[deviceManagementReportSchedule](../resources/deviceManagementReportSchedule.md) collection|Get the deviceManagementReportSchedules from the reportSchedules navigation property.|
|[Add reportSchedules](../api/devicemanagementreports-post-reportschedules.md)|[deviceManagementReportSchedule](../resources/deviceManagementReportSchedule.md)|Add reportSchedules by posting to the reportSchedules collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|cachedReportConfigurations|[deviceManagementCachedReportConfiguration](../resources/deviceManagementCachedReportConfiguration.md) collection|Entity representing the configuration of a cached report|
|exportJobs|[deviceManagementExportJob](../resources/deviceManagementExportJob.md) collection|Entity representing a job to export a report|
|reportSchedules|[deviceManagementReportSchedule](../resources/deviceManagementReportSchedule.md) collection|Entity representing a schedule for which reports are delivered|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReports",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "String (identifier)"
}
```

