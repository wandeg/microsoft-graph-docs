---
title: "workbookTableColumn resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookTableColumn resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[dataBodyRange](../api/workbooktablecolumn-databodyrange.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[headerRowRange](../api/workbooktablecolumn-headerrowrange.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[range](../api/workbooktablecolumn-range.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[totalRowRange](../api/workbooktablecolumn-totalrowrange.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[add](../api/workbooktablecolumn-add.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|**TODO: Add Description**|
|[itemAt](../api/workbooktablecolumn-itemat.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|**TODO: Add Description**|
|[count](../api/workbooktablecolumn-count.md)|Int32|**TODO: Add Description**|
|[List filter](../api/workbooktablecolumn-list-filter.md)|[workbookFilter](../resources/workbookfilter.md) collection|Get the workbookFilters from the filter navigation property.|
|[Create filter](../api/workbooktablecolumn-post-filter.md)|[workbookFilter](../resources/workbookfilter.md)|Create a new filter object.|
|[Delete filter](../api/workbooktablecolumn-delete-filter.md)|None|Delete a [workbookFilter](../resources/workbookfilter.md) object.|
|[Update filter](../api/workbooktablecolumn-update-filter.md)|[workbookFilter](../resources/workbookfilter.md)|Update the properties of a filter object.|
|[Get workbookFilter](../api/workbookfilter-get.md)|[workbookFilter](../resources/workbookfilter.md)|Read the properties and relationships of a [workbookFilter](../resources/workbookfilter.md) object.|
|[List columns](../api/workbooktable-list-columns.md)|[workbookTableColumn](../resources/workbooktablecolumn.md) collection|Get the workbookTableColumns from the columns navigation property.|
|[Create columns](../api/workbooktable-post-columns.md)|[workbookTableColumn](../resources/workbooktablecolumn.md)|Create a new columns object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|index|Int32|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|values|[Json](../resources/json.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|filter|[workbookFilter](../resources/workbookfilter.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookTableColumn",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTableColumn",
  "id": "String (identifier)",
  "index": "Integer",
  "name": "String",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

