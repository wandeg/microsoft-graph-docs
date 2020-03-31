---
title: "deviceManagementReports resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementReports resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementReports](../api/devicemanagementreports-get.md)|[deviceManagementReports](../resources/devicemanagementreports.md)|Read properties and relationships of the [deviceManagementReports](../resources/devicemanagementreports.md) object.|
|[Update deviceManagementReports](../api/devicemanagementreports-update.md)|[deviceManagementReports](../resources/devicemanagementreports.md)|Update the properties of a [deviceManagementReports](../resources/devicemanagementreports.md) object.|
|[getDeviceNonComplianceReport](../api/devicemanagementreports-getdevicenoncompliancereport.md)|Stream||
|[getPolicyNonComplianceReport](../api/devicemanagementreports-getpolicynoncompliancereport.md)|Stream||
|[getPolicyNonComplianceMetadata](../api/devicemanagementreports-getpolicynoncompliancemetadata.md)|Stream||
|[getSettingNonComplianceReport](../api/devicemanagementreports-getsettingnoncompliancereport.md)|Stream||
|[getHistoricalReport](../api/devicemanagementreports-gethistoricalreport.md)|Stream||
|[getCachedReport](../api/devicemanagementreports-getcachedreport.md)|Stream||
|[List cachedReportConfigurations](../api/devicemanagementreports-list-cachedreportconfigurations.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) collection|Get the deviceManagementCachedReportConfigurations from the cachedReportConfigurations navigation property.|
|[Add cachedReportConfigurations](../api/devicemanagementreports-post-cachedreportconfigurations.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Add cachedReportConfigurations by posting to the cachedReportConfigurations collection.|
|[List exportJobs](../api/devicemanagementreports-list-exportjobs.md)|[deviceManagementExportJob](../resources/devicemanagementexportjob.md) collection|Get the deviceManagementExportJobs from the exportJobs navigation property.|
|[Add exportJobs](../api/devicemanagementreports-post-exportjobs.md)|[deviceManagementExportJob](../resources/devicemanagementexportjob.md)|Add exportJobs by posting to the exportJobs collection.|
|[List reportSchedules](../api/devicemanagementreports-list-reportschedules.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) collection|Get the deviceManagementReportSchedules from the reportSchedules navigation property.|
|[Add reportSchedules](../api/devicemanagementreports-post-reportschedules.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Add reportSchedules by posting to the reportSchedules collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|cachedReportConfigurations|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) collection||
|exportJobs|[deviceManagementExportJob](../resources/devicemanagementexportjob.md) collection||
|reportSchedules|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) collection||

## JSON representation
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

