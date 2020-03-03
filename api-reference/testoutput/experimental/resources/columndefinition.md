---
title: "columnDefinition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# columnDefinition resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get columnDefinition](../api/columndefinition-get.md)|[columnDefinition](../resources/columnDefinition.md)|Read properties and relationships of the [columnDefinition](../resources/columndefinition.md) object.|
|[Delete columnDefinition](../api/columndefinition-delete.md)|None|Deletes a [columnDefinition](../resources/columndefinition.md).|
|[Update columnDefinition](../api/columndefinition-update.md)|[columnDefinition](../resources/columnDefinition.md)|Update the properties of a [columnDefinition](../resources/columndefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|boolean|[booleanColumn](../resources/booleanColumn.md)||
|calculated|[calculatedColumn](../resources/calculatedColumn.md)||
|choice|[choiceColumn](../resources/choiceColumn.md)||
|columnGroup|String||
|currency|[currencyColumn](../resources/currencyColumn.md)||
|dateTime|[dateTimeColumn](../resources/dateTimeColumn.md)||
|defaultValue|[defaultColumnValue](../resources/defaultColumnValue.md)||
|description|String||
|displayName|String||
|enforceUniqueValues|Boolean||
|geolocation|[geolocationColumn](../resources/geolocationColumn.md)||
|hidden|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|indexed|Boolean||
|lookup|[lookupColumn](../resources/lookupColumn.md)||
|name|String||
|number|[numberColumn](../resources/numberColumn.md)||
|personOrGroup|[personOrGroupColumn](../resources/personOrGroupColumn.md)||
|readOnly|Boolean||
|required|Boolean||
|text|[textColumn](../resources/textColumn.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.columnDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.columnDefinition",
  "id": "String (identifier)",
  "boolean": {
    "@odata.type": "microsoft.graph.booleanColumn"
  },
  "calculated": {
    "@odata.type": "microsoft.graph.calculatedColumn"
  },
  "choice": {
    "@odata.type": "microsoft.graph.choiceColumn"
  },
  "columnGroup": "String",
  "currency": {
    "@odata.type": "microsoft.graph.currencyColumn"
  },
  "dateTime": {
    "@odata.type": "microsoft.graph.dateTimeColumn"
  },
  "defaultValue": {
    "@odata.type": "microsoft.graph.defaultColumnValue"
  },
  "description": "String",
  "displayName": "String",
  "enforceUniqueValues": true,
  "geolocation": {
    "@odata.type": "microsoft.graph.geolocationColumn"
  },
  "hidden": true,
  "indexed": true,
  "lookup": {
    "@odata.type": "microsoft.graph.lookupColumn"
  },
  "name": "String",
  "number": {
    "@odata.type": "microsoft.graph.numberColumn"
  },
  "personOrGroup": {
    "@odata.type": "microsoft.graph.personOrGroupColumn"
  },
  "readOnly": true,
  "required": true,
  "text": {
    "@odata.type": "microsoft.graph.textColumn"
  }
}
```

