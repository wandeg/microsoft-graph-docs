---
title: "printDocument resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printDocument resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printDocument](../api/printdocument-get.md)|[printDocument](../resources/printdocument.md)|Read properties and relationships of the [printDocument](../resources/printdocument.md) object.|
|[Update printDocument](../api/printdocument-update.md)|[printDocument](../resources/printdocument.md)|Update the properties of a [printDocument](../resources/printdocument.md) object.|
|[uploadData](../api/printdocument-uploaddata.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|documentConfiguration|[printerDocumentConfiguration](../resources/printerdocumentconfiguration.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|mimeType|String||
|name|String||
|sizeInBytes|Int64||

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

