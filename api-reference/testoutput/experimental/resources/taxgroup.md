---
title: "taxGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# taxGroup resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List taxGroups](../api/taxgroup-list.md)|[taxGroup](../resources/taxgroup.md) collection|List properties and relationships of the [taxGroup](../resources/taxgroup.md) objects.|
|[Get taxGroup](../api/taxgroup-get.md)|[taxGroup](../resources/taxgroup.md)|Read properties and relationships of the [taxGroup](../resources/taxgroup.md) object.|
|[Create taxGroup](../api/taxgroup-create.md)|[taxGroup](../resources/taxgroup.md)|Create a new [taxGroup](../resources/taxgroup.md) object.|
|[Delete taxGroup](../api/taxgroup-delete.md)|None|Deletes a [taxGroup](../resources/taxgroup.md).|
|[Update taxGroup](../api/taxgroup-update.md)|[taxGroup](../resources/taxgroup.md)|Update the properties of a [taxGroup](../resources/taxgroup.md) object.|

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
  "@odata.type": "microsoft.graph.taxGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taxGroup",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

