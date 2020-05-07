---
title: "deviceManagementReportSchedule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementReportSchedule resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|emails|String collection|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|filter|String|**TODO: Add Description**|
|format|deviceManagementReportFileFormat|**TODO: Add Description**. Possible values are: `csv`, `pdf`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|orderBy|String collection|**TODO: Add Description**|
|recurrence|deviceManagementScheduledReportRecurrence|**TODO: Add Description**. Possible values are: `none`, `daily`, `weekly`, `monthly`.|
|reportName|String|**TODO: Add Description**|
|reportScheduleName|String|**TODO: Add Description**|
|select|String collection|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

