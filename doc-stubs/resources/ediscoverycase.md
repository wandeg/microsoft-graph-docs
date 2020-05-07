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

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List ediscoveryCases](../api/ediscoverycase-list.md)|[ediscoveryCase](../resources/ediscoverycase.md) collection|Get a list of the [ediscoveryCase](../resources/ediscoverycase.md) objects and their properties.|
|[Get ediscoveryCase](../api/ediscoverycase-get.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Read the properties and relationships of an [ediscoveryCase](../resources/ediscoverycase.md) object.|
|[Create ediscoveryCase](../api/ediscoverycase-post-cases.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Create a new [ediscoveryCase](../resources/ediscoverycase.md) object.|
|[Delete ediscoveryCase](../api/ediscoverycase-delete.md)|None|Deletes an [ediscoveryCase](../resources/ediscoverycase.md) object.|
|[Update ediscoveryCase](../api/ediscoverycase-update.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Update the properties of an [ediscoveryCase](../resources/ediscoverycase.md) object.|
|[List reviewSets](../api/ediscoverycase-list-reviewsets.md)|[reviewSet](../resources/reviewset.md) collection|Get the reviewSets from the reviewSets navigation property.|
|[Create reviewSets](../api/ediscoverycase-post-reviewsets.md)|[reviewSet](../resources/reviewset.md)|Create a new reviewSets object.|
|[Delete reviewSets](../api/ediscoverycase-delete-reviewsets.md)|None|Delete a [reviewSet](../resources/reviewset.md) object.|
|[Update reviewSets](../api/ediscoverycase-update-reviewsets.md)|[reviewSet](../resources/reviewset.md)|Update the properties of a reviewSets object.|
|[Get reviewSet](../api/reviewset-get.md)|[reviewSet](../resources/reviewset.md)|Read the properties and relationships of a [reviewSet](../resources/reviewset.md) object.|

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
|id|String|**TODO: Add Description**|
|lastModifiedBy|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|caseStatus|**TODO: Add Description**. Possible values are: `unknown`, `active`, `pendingDelete`, `closing`, `closed`, `closedWithError`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|reviewSets|[reviewSet](../resources/reviewset.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.compliance.ediscovery.contract.ediscoveryCase",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.compliance.ediscovery.contract.ediscoveryCase",
  "description": "String",
  "createdBy": "String",
  "lastModifiedBy": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": "String",
  "closedDateTime": "String (timestamp)",
  "externalId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

