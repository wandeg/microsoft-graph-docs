---
title: "unitOfMeasure resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# unitOfMeasure resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get unitOfMeasure](../api/unitofmeasure-get.md)|[unitOfMeasure](../resources/unitOfMeasure.md)|Read properties and relationships of the [unitOfMeasure](../resources/unitofmeasure.md) object.|
|[Delete unitOfMeasure](../api/unitofmeasure-delete.md)|None|Deletes a [unitOfMeasure](../resources/unitofmeasure.md).|
|[Update unitOfMeasure](../api/unitofmeasure-update.md)|[unitOfMeasure](../resources/unitOfMeasure.md)|Update the properties of a [unitOfMeasure](../resources/unitofmeasure.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|internationalStandardCode|String||
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unitOfMeasure",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unitOfMeasure",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "internationalStandardCode": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

