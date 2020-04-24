---
title: "workbookTableRow resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookTableRow resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookTableRow](../api/workbooktablerow-get.md)|[workbookTableRow](../resources/workbooktablerow.md)|Read the properties and relationships of a [workbookTableRow](../resources/workbooktablerow.md) object.|
|[Update workbookTableRow](../api/workbooktablerow-update.md)|[workbookTableRow](../resources/workbooktablerow.md)|Update the properties of a [workbookTableRow](../resources/workbooktablerow.md) object.|
|[range](../api/workbooktablerow-range.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[add](../api/workbooktablerow-add.md)|[workbookTableRow](../resources/workbooktablerow.md)|**TODO: Add Description**|
|[itemAt](../api/workbooktablerow-itemat.md)|[workbookTableRow](../resources/workbooktablerow.md)|**TODO: Add Description**|
|[count](../api/workbooktablerow-count.md)|Int32|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|index|Int32|**TODO: Add Description**|
|values|[Json](../resources/json.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookTableRow",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTableRow",
  "id": "String (identifier)",
  "index": 1024,
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

