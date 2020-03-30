---
title: "deviceManagementReportSchedule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementReportSchedule resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementReportSchedule](../api/devicemanagementreportschedule-get.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Read properties and relationships of the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.|
|[Update deviceManagementReportSchedule](../api/devicemanagementreportschedule-update.md)|[deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md)|Update the properties of a [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|emails|String collection||
|endDateTime|DateTimeOffset||
|filter|String||
|format|Enumeration| Possible values are: `csv`, `pdf`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|orderBy|String collection||
|recurrence|Enumeration| Possible values are: `none`, `daily`, `weekly`, `monthly`.|
|reportName|String||
|reportScheduleName|String||
|select|String collection||
|startDateTime|DateTimeOffset||
|subject|String||
|userId|String||

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

