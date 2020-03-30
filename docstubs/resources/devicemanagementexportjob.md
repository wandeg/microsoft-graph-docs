---
title: "deviceManagementExportJob resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementExportJob resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementExportJob](../api/devicemanagementexportjob-get.md)|[deviceManagementExportJob](../resources/devicemanagementexportjob.md)|Read properties and relationships of the [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.|
|[Update deviceManagementExportJob](../api/devicemanagementexportjob-update.md)|[deviceManagementExportJob](../resources/devicemanagementexportjob.md)|Update the properties of a [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expirationDateTime|DateTimeOffset||
|filter|String||
|format|Enumeration| Possible values are: `csv`, `pdf`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportName|String||
|requestDateTime|DateTimeOffset||
|select|String collection||
|snapshotId|String||
|status|Enumeration| Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|String||

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

