---
title: "reviewSet resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# reviewSet resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List queries](../api/reviewset-list-queries.md)|[reviewSetQuery](../resources/reviewsetquery.md) collection|Get the reviewSetQueries from the queries navigation property.|
|[Create queries](../api/reviewset-post-queries.md)|[reviewSetQuery](../resources/reviewsetquery.md)|Create a new queries object.|
|[Delete queries](../api/reviewset-delete-queries.md)|None|Delete a [reviewSetQuery](../resources/reviewsetquery.md) object.|
|[Update queries](../api/reviewset-update-queries.md)|[reviewSetQuery](../resources/reviewsetquery.md)|Update the properties of a queries object.|
|[Get reviewSetQuery](../api/reviewsetquery-get.md)|[reviewSetQuery](../resources/reviewsetquery.md)|Read the properties and relationships of a [reviewSetQuery](../resources/reviewsetquery.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|queries|[reviewSetQuery](../resources/reviewsetquery.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reviewSet",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reviewSet",
  "id": "String (identifier)",
  "createdBy": "String",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

