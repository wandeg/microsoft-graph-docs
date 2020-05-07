---
title: "printJob resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printJob resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[cancelPrintJob](../api/printjob-cancelprintjob.md)|None|**TODO: Add Description**|
|[startPrintJob](../api/printjob-startprintjob.md)|[printJobStatus](../resources/printjobstatus.md)|**TODO: Add Description**|
|[List documents](../api/printjob-list-documents.md)|[printDocument](../resources/printdocument.md) collection|Get the printDocuments from the documents navigation property.|
|[Create documents](../api/printjob-post-documents.md)|[printDocument](../resources/printdocument.md)|Create a new documents object.|
|[Delete documents](../api/printjob-delete-documents.md)|None|Delete a [printDocument](../resources/printdocument.md) object.|
|[Update documents](../api/printjob-update-documents.md)|[printDocument](../resources/printdocument.md)|Update the properties of a documents object.|
|[Get printDocument](../api/printdocument-get.md)|[printDocument](../resources/printdocument.md)|Read the properties and relationships of a [printDocument](../resources/printdocument.md) object.|
|[List jobs](../api/printer-list-jobs.md)|[printJob](../resources/printjob.md) collection|Get the printJobs from the jobs navigation property.|
|[Create jobs](../api/printer-post-jobs.md)|[printJob](../resources/printjob.md)|Create a new jobs object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|[printJobStatus](../resources/printjobstatus.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|documents|[printDocument](../resources/printdocument.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.printJobStatus"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  }
}
```

