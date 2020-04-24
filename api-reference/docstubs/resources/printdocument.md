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


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printDocument](../api/printdocument-get.md)|[printDocument](../resources/printdocument.md)|Read the properties and relationships of a [printDocument](../resources/printdocument.md) object.|
|[Update printDocument](../api/printdocument-update.md)|[printDocument](../resources/printdocument.md)|Update the properties of a [printDocument](../resources/printdocument.md) object.|
|[uploadData](../api/printdocument-uploaddata.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|documentConfiguration|[printerDocumentConfiguration](../resources/printerdocumentconfiguration.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|mimeType|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|sizeInBytes|Int64|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "sizeInBytes": 1024,
  "documentConfiguration": {
    "@odata.type": "microsoft.graph.printerDocumentConfiguration"
  }
}
```

