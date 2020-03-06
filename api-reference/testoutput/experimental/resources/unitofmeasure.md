---
title: "unitOfMeasure resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# unitOfMeasure resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get unitOfMeasure](../api/unitofmeasure-get.md)|[unitOfMeasure](../resources/unitofmeasure.md)|Read properties and relationships of the [unitOfMeasure](../resources/unitofmeasure.md) object.|
|[Update unitOfMeasure](../api/unitofmeasure-update.md)|[unitOfMeasure](../resources/unitofmeasure.md)|Update the properties of a [unitOfMeasure](../resources/unitofmeasure.md) object.|
|[List unitsOfMeasure](../api/company-list-unitsofmeasure.md)|[unitOfMeasure](../resources/unitofmeasure.md) collection|Get the unitOfMeasures from the unitsOfMeasure navigation property.|
|[Add unitsOfMeasure](../api/company-post-unitsofmeasure.md)|[unitOfMeasure](../resources/unitofmeasure.md)|Add unitsOfMeasure by posting to the unitsOfMeasure collection.|

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

## JSON representation
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

