---
title: "taxArea resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# taxArea resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get taxArea](../api/taxarea-get.md)|[taxArea](../resources/taxArea.md)|Read properties and relationships of the [taxArea](../resources/taxarea.md) object.|
|[Delete taxArea](../api/taxarea-delete.md)|None|Deletes a [taxArea](../resources/taxarea.md).|
|[Update taxArea](../api/taxarea-update.md)|[taxArea](../resources/taxArea.md)|Update the properties of a [taxArea](../resources/taxarea.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|taxType|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.taxArea",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taxArea",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

