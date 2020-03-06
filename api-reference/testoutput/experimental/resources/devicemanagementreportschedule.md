---
title: "deviceManagementReportSchedule resource type"
description: "Entity representing a schedule for which reports are delivered"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementReportSchedule resource type


Namespace: microsoft.graph

Entity representing a schedule for which reports are delivered


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementReportSchedule](../api/devicemanagementreportschedule-get.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Read properties and relationships of the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.|
|[Update deviceManagementReportSchedule](../api/devicemanagementreportschedule-update.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Update the properties of a [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.|
|[List reportSchedules](../api/devicemanagementreports-list-reportschedules.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) collection|Get the deviceManagementReportSchedules from the reportSchedules navigation property.|
|[Add reportSchedules](../api/devicemanagementreports-post-reportschedules.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Add reportSchedules by posting to the reportSchedules collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|emails|String collection|Emails to which the scheduled reports are delivered|
|endDateTime|DateTimeOffset|Time that the delivery of the scheduled reports ends|
|filter|String|Filters applied on the report|
|format|Enumeration|Format of the scheduled report. Possible values are: `csv`, `pdf`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|orderBy|String collection|Ordering of columns in the report|
|recurrence|Enumeration|Frequency of scheduled report delivery. Possible values are: `none`, `daily`, `weekly`, `monthly`.|
|reportName|String|Name of the report|
|reportScheduleName|String|Name of the schedule|
|select|String collection|Columns selected from the report|
|startDateTime|DateTimeOffset|Time that the delivery of the scheduled reports starts|
|subject|String|Subject of the scheduled reports that are delivered|
|userId|String|The Id of the User who created the report|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReportSchedule",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "String (identifier)",
  "reportScheduleName": "String",
  "subject": "String",
  "emails": [
    "String"
  ],
  "recurrence": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "userId": "String",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "format": "String"
}
```

