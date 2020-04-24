---
title: "ediscoveryCase resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# ediscoveryCase resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List ediscoveryCases](../api/ediscoverycase-list.md)|[ediscoveryCase](../resources/ediscoverycase.md) collection|Get a list of the [ediscoveryCase](../resources/ediscoverycase.md) objects and their properties.|
|[Get ediscoveryCase](../api/ediscoverycase-get.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Read the properties and relationships of an [ediscoveryCase](../resources/ediscoverycase.md) object.|
|[Create ediscoveryCase](../api/ediscoverycase-post-cases.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Create a new [ediscoveryCase](../resources/ediscoverycase.md) object.|
|[Delete ediscoveryCase](../api/ediscoverycase-delete.md)|None|Deletes an [ediscoveryCase](../resources/ediscoverycase.md) object.|
|[Update ediscoveryCase](../api/ediscoverycase-update.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Update the properties of an [ediscoveryCase](../resources/ediscoverycase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|closedBy|String|**TODO: Add Description**|
|closedDateTime|DateTimeOffset|**TODO: Add Description**|
|createdBy|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|caseStatus|**TODO: Add Description**. Possible values are: `unknown`, `active`, `pendingDelete`, `closing`, `closed`, `closedWithError`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscoveryCase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "id": "String (identifier)",
  "description": "String",
  "createdBy": "String",
  "lastModifiedBy": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": "String",
  "closedDateTime": "String (timestamp)",
  "externalId": "String",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

