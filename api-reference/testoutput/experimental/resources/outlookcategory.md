---
title: "outlookCategory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# outlookCategory resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get outlookCategory](../api/outlookcategory-get.md)|[outlookCategory](../resources/outlookCategory.md)|Read properties and relationships of the [outlookCategory](../resources/outlookcategory.md) object.|
|[Delete outlookCategory](../api/outlookcategory-delete.md)|None|Deletes a [outlookCategory](../resources/outlookcategory.md).|
|[Update outlookCategory](../api/outlookcategory-update.md)|[outlookCategory](../resources/outlookCategory.md)|Update the properties of a [outlookCategory](../resources/outlookcategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|Enumeration|. Possible values are: `preset0`, `preset1`, `preset2`, `preset3`, `preset4`, `preset5`, `preset6`, `preset7`, `preset8`, `preset9`, `preset10`, `preset11`, `preset12`, `preset13`, `preset14`, `preset15`, `preset16`, `preset17`, `preset18`, `preset19`, `preset20`, `preset21`, `preset22`, `preset23`, `preset24`, `none`.|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.outlookCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outlookCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "color": "String"
}
```

