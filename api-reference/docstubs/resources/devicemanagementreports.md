---
title: "deviceManagementReports resource type"
description: "Singleton entity that acts as a container for all reports functionality."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementReports resource type


Namespace: microsoft.graph

Singleton entity that acts as a container for all reports functionality.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementReports](../api/devicemanagementreports-get.md)|[deviceManagementReports](../resources/devicemanagementreports.md)|Read the properties and relationships of a [deviceManagementReports](../resources/devicemanagementreports.md) object.|
|[Update deviceManagementReports](../api/devicemanagementreports-update.md)|[deviceManagementReports](../resources/devicemanagementreports.md)|Update the properties of a [deviceManagementReports](../resources/devicemanagementreports.md) object.|
|[getDeviceNonComplianceReport](../api/devicemanagementreports-getdevicenoncompliancereport.md)|Stream|**TODO: Add Description**|
|[getPolicyNonComplianceReport](../api/devicemanagementreports-getpolicynoncompliancereport.md)|Stream|**TODO: Add Description**|
|[getPolicyNonComplianceMetadata](../api/devicemanagementreports-getpolicynoncompliancemetadata.md)|Stream|**TODO: Add Description**|
|[getPolicyNonComplianceSummaryReport](../api/devicemanagementreports-getpolicynoncompliancesummaryreport.md)|Stream|**TODO: Add Description**|
|[getSettingNonComplianceReport](../api/devicemanagementreports-getsettingnoncompliancereport.md)|Stream|**TODO: Add Description**|
|[getHistoricalReport](../api/devicemanagementreports-gethistoricalreport.md)|Stream|**TODO: Add Description**|
|[getCachedReport](../api/devicemanagementreports-getcachedreport.md)|Stream|**TODO: Add Description**|
|[getWindowsUpdateAlertSummaryReport](../api/devicemanagementreports-getwindowsupdatealertsummaryreport.md)|Stream|**TODO: Add Description**|
|[getWindowsUpdateAlertsPerPolicyPerDeviceReport](../api/devicemanagementreports-getwindowsupdatealertsperpolicyperdevicereport.md)|Stream|**TODO: Add Description**|
|[List cachedReportConfigurations](../api/devicemanagementreports-list-cachedreportconfigurations.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) collection|Get the deviceManagementCachedReportConfigurations from the cachedReportConfigurations navigation property.|
|[Create cachedReportConfigurations](../api/devicemanagementreports-post-cachedreportconfigurations.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Create a new cachedReportConfigurations object.|
|[Delete cachedReportConfigurations](../api/devicemanagementreports-delete-cachedreportconfigurations.md)|None|Delete a [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.|
|[Update cachedReportConfigurations](../api/devicemanagementreports-update-cachedreportconfigurations.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Update the properties of a cachedReportConfigurations object.|
|[Get deviceManagementCachedReportConfiguration](../api/devicemanagementcachedreportconfiguration-get.md)|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md)|Read the properties and relationships of a [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.|
|[List exportJobs](../api/devicemanagementreports-list-exportjobs.md)|[deviceManagementExportJob](../resources/devicemanagementexportjob.md) collection|Get the deviceManagementExportJobs from the exportJobs navigation property.|
|[Create exportJobs](../api/devicemanagementreports-post-exportjobs.md)|[deviceManagementExportJob](../resources/devicemanagementexportjob.md)|Create a new exportJobs object.|
|[Delete exportJobs](../api/devicemanagementreports-delete-exportjobs.md)|None|Delete an [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.|
|[Update exportJobs](../api/devicemanagementreports-update-exportjobs.md)|[deviceManagementExportJob](../resources/devicemanagementexportjob.md)|Update the properties of an exportJobs object.|
|[Get deviceManagementExportJob](../api/devicemanagementexportjob-get.md)|[deviceManagementExportJob](../resources/devicemanagementexportjob.md)|Read the properties and relationships of a [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.|
|[List reportSchedules](../api/devicemanagementreports-list-reportschedules.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) collection|Get the deviceManagementReportSchedules from the reportSchedules navigation property.|
|[Create reportSchedules](../api/devicemanagementreports-post-reportschedules.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Create a new reportSchedules object.|
|[Delete reportSchedules](../api/devicemanagementreports-delete-reportschedules.md)|None|Delete a [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.|
|[Update reportSchedules](../api/devicemanagementreports-update-reportschedules.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Update the properties of a reportSchedules object.|
|[Get deviceManagementReportSchedule](../api/devicemanagementreportschedule-get.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Read the properties and relationships of a [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|cachedReportConfigurations|[deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) collection|Entity representing the configuration of a cached report|
|exportJobs|[deviceManagementExportJob](../resources/devicemanagementexportjob.md) collection|Entity representing a job to export a report|
|reportSchedules|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) collection|Entity representing a schedule for which reports are delivered|

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

