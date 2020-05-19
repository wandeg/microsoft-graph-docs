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


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List rows](../api/workbooktable-list-rows.md)|[workbookTableRow](../resources/workbooktablerow.md) collection|Get the workbookTableRows from the rows navigation property.|
|[Create rows](../api/workbooktable-post-rows.md)|[workbookTableRow](../resources/workbooktablerow.md)|Create a new rows object.|
|[Delete rows](../api/workbooktable-delete-rows.md)|None|Delete a [workbookTableRow](../resources/workbooktablerow.md) object.|
|[Update rows](../api/workbooktable-update-rows.md)|[workbookTableRow](../resources/workbooktablerow.md)|Update the properties of a rows object.|
|[Get rows](../api/workbooktable-get-workbooktablerow.md)|[workbookTableRow](../resources/workbooktablerow.md)|Read the properties and relationships of a [workbookTableRow](../resources/workbooktablerow.md) object.|
|[range](../api/workbooktablerow-range.md)|[workbookRange](../resources/workbookrange.md)|**TODO: Add Description**|
|[add](../api/workbooktablerow-add.md)|[workbookTableRow](../resources/workbooktablerow.md)|**TODO: Add Description**|
|[itemAt](../api/workbooktablerow-itemat.md)|[workbookTableRow](../resources/workbooktablerow.md)|**TODO: Add Description**|
|[count](../api/workbooktablerow-count.md)|Int32|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|index|Int32|**TODO: Add Description**|
|values|[Json](../resources/intune-json.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "index": "Integer",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

