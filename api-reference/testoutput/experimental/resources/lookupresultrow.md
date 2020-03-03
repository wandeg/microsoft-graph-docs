---
title: "lookupResultRow resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# lookupResultRow resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get lookupResultRow](../api/lookupresultrow-get.md)|[lookupResultRow](../resources/lookupResultRow.md)|Read properties and relationships of the [lookupResultRow](../resources/lookupresultrow.md) object.|
|[Delete lookupResultRow](../api/lookupresultrow-delete.md)|None|Deletes a [lookupResultRow](../resources/lookupresultrow.md).|
|[Update lookupResultRow](../api/lookupresultrow-update.md)|[lookupResultRow](../resources/lookupResultRow.md)|Update the properties of a [lookupResultRow](../resources/lookupresultrow.md) object.|
|[List matchingRows](../api/exactmatchlookupjob-list-matchingrows.md)|[lookupResultRow](../resources/lookupResultRow.md) collection|Get the lookupResultRows from the matchingRows navigation property.|
|[Add matchingRows](../api/exactmatchlookupjob-post-matchingrows.md)|[lookupResultRow](../resources/lookupResultRow.md)|Add matchingRows by posting to the matchingRows collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|row|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.lookupResultRow",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.lookupResultRow",
  "id": "String (identifier)",
  "row": "String"
}
```

