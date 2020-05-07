---
title: "printDocument resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printDocument resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[uploadData](../api/printdocument-uploaddata.md)|None|**TODO: Add Description**|
|[List documents](../api/printjob-list-documents.md)|[printDocument](../resources/printdocument.md) collection|Get the printDocuments from the documents navigation property.|
|[Create documents](../api/printjob-post-documents.md)|[printDocument](../resources/printdocument.md)|Create a new documents object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|documentConfiguration|[printerDocumentConfiguration](../resources/printerdocumentconfiguration.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|mimeType|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|sizeInBytes|Int64|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printDocument",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocument",
  "id": "String (identifier)",
  "name": "String",
  "mimeType": "String",
  "sizeInBytes": "Integer",
  "documentConfiguration": {
    "@odata.type": "microsoft.graph.printerDocumentConfiguration"
  }
}
```

