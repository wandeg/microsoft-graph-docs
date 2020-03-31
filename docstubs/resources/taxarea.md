---
title: "taxArea resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# taxArea resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get taxArea](../api/taxarea-get.md)|[taxArea](../resources/taxarea.md)|Read properties and relationships of the [taxArea](../resources/taxarea.md) object.|
|[Update taxArea](../api/taxarea-update.md)|[taxArea](../resources/taxarea.md)|Update the properties of a [taxArea](../resources/taxarea.md) object.|
|[List taxAreas](../api/company-list-taxareas.md)|[taxArea](../resources/taxarea.md) collection|Get the taxAreas from the taxAreas navigation property.|
|[Add taxAreas](../api/company-post-taxareas.md)|[taxArea](../resources/taxarea.md)|Add taxAreas by posting to the taxAreas collection.|

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

## JSON representation
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

