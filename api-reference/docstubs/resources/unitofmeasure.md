---
title: "unitOfMeasure resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# unitOfMeasure resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get unitOfMeasure](../api/unitofmeasure-get.md)|[unitOfMeasure](../resources/unitofmeasure.md)|Read the properties and relationships of an [unitOfMeasure](../resources/unitofmeasure.md) object.|
|[Update unitOfMeasure](../api/unitofmeasure-update.md)|[unitOfMeasure](../resources/unitofmeasure.md)|Update the properties of an [unitOfMeasure](../resources/unitofmeasure.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|internationalStandardCode|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

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

