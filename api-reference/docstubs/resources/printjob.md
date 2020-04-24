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


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printJob](../api/printjob-get.md)|[printJob](../resources/printjob.md)|Read the properties and relationships of a [printJob](../resources/printjob.md) object.|
|[Update printJob](../api/printjob-update.md)|[printJob](../resources/printjob.md)|Update the properties of a [printJob](../resources/printjob.md) object.|
|[cancelPrintJob](../api/printjob-cancelprintjob.md)|None|**TODO: Add Description**|
|[startPrintJob](../api/printjob-startprintjob.md)|[printJobStatus](../resources/printjobstatus.md)|**TODO: Add Description**|
|[List documents](../api/printjob-list-documents.md)|[printDocument](../resources/printdocument.md) collection|Get the printDocuments from the documents navigation property.|
|[Create documents](../api/printjob-post-documents.md)|[printDocument](../resources/printdocument.md)|Create a new documents object.|
|[Delete documents](../api/printjob-delete-documents.md)|None|Delete a [printDocument](../resources/printdocument.md) object.|
|[Update documents](../api/printjob-update-documents.md)|[printDocument](../resources/printdocument.md)|Update the properties of a documents object.|
|[Get printDocument](../api/printdocument-get.md)|[printDocument](../resources/printdocument.md)|Read the properties and relationships of a [printDocument](../resources/printdocument.md) object.|

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

