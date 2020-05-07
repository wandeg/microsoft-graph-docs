---
title: "deviceManagementExportJob resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementExportJob resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|filter|String|**TODO: Add Description**|
|format|deviceManagementReportFileFormat|**TODO: Add Description**. Possible values are: `csv`, `pdf`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|reportName|String|**TODO: Add Description**|
|requestDateTime|DateTimeOffset|**TODO: Add Description**|
|select|String collection|**TODO: Add Description**|
|snapshotId|String|**TODO: Add Description**|
|status|deviceManagementReportStatus|**TODO: Add Description**. Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

