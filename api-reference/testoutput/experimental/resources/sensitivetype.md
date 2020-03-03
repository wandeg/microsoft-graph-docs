---
title: "sensitiveType resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sensitiveType resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sensitiveTypes](../api/sensitivetype-list.md)|[sensitiveType](../resources/sensitivetype.md) collection|List properties and relationships of the [sensitiveType](../resources/sensitivetype.md) objects.|
|[Get sensitiveType](../api/sensitivetype-get.md)|[sensitiveType](../resources/sensitivetype.md)|Read properties and relationships of the [sensitiveType](../resources/sensitivetype.md) object.|
|[Create sensitiveType](../api/sensitivetype-create.md)|[sensitiveType](../resources/sensitivetype.md)|Create a new [sensitiveType](../resources/sensitivetype.md) object.|
|[Delete sensitiveType](../api/sensitivetype-delete.md)|None|Deletes a [sensitiveType](../resources/sensitivetype.md).|
|[Update sensitiveType](../api/sensitivetype-update.md)|[sensitiveType](../resources/sensitivetype.md)|Update the properties of a [sensitiveType](../resources/sensitivetype.md) object.|
|[List sensitiveTypes](../api/dataclassificationservice-list-sensitivetypes.md)|[sensitiveType](../resources/sensitivetype.md) collection|Get the sensitiveTypes from the sensitiveTypes navigation property.|
|[Add sensitiveTypes](../api/dataclassificationservice-post-sensitivetypes.md)|[sensitiveType](../resources/sensitivetype.md)|Add sensitiveTypes by posting to the sensitiveTypes collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|publisherName|String||
|rulePackageId|String||
|rulePackageType|String||
|scope|Enumeration|. Possible values are: `fullDocument`, `partialDocument`.|
|state|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sensitiveType",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sensitiveType",
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "rulePackageId": "String",
  "rulePackageType": "String",
  "publisherName": "String",
  "state": "String",
  "scope": "String"
}
```

