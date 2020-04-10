---
title: "printJob resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printJob resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printJob](../api/printjob-get.md)|[printJob](../resources/printjob.md)|Read properties and relationships of the [printJob](../resources/printjob.md) object.|
|[Update printJob](../api/printjob-update.md)|[printJob](../resources/printjob.md)|Update the properties of a [printJob](../resources/printjob.md) object.|
|[cancelPrintJob](../api/printjob-cancelprintjob.md)|None||
|[startPrintJob](../api/printjob-startprintjob.md)|[printJobStatus](../resources/printjobstatus.md)||
|[List documents](../api/printjob-list-documents.md)|[printDocument](../resources/printdocument.md) collection|Get the printDocuments from the documents navigation property.|
|[Add documents](../api/printjob-post-documents.md)|[printDocument](../resources/printdocument.md)|Add documents by posting to the documents collection.|
|[List jobs](../api/printer-list-jobs.md)|[printJob](../resources/printjob.md) collection|Get the printJobs from the jobs navigation property.|
|[Add jobs](../api/printer-post-jobs.md)|[printJob](../resources/printjob.md)|Add jobs by posting to the jobs collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[userIdentity](../resources/useridentity.md)||
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|status|[printJobStatus](../resources/printjobstatus.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|documents|[printDocument](../resources/printdocument.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printJob",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJob",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "status": {
    "@odata.type": "microsoft.graph.printJobStatus",
    "processingState": "String",
    "processingStateDescription": "String",
    "acquiredByPrinter": true
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity",
    "id": "String",
    "displayName": "String",
    "ipAddress": "String",
    "userPrincipalName": "String"
  }
}
```

