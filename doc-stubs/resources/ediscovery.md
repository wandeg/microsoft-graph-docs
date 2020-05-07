---
title: "ediscovery resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# ediscovery resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List cases](../api/ediscovery-list-cases.md)|[ediscoveryCase](../resources/ediscoverycase.md) collection|Get the ediscoveryCases from the cases navigation property.|
|[Create cases](../api/ediscovery-post-cases.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Create a new cases object.|
|[Delete cases](../api/ediscovery-delete-cases.md)|None|Delete a [ediscoveryCase](../resources/ediscoverycase.md) object.|
|[Update cases](../api/ediscovery-update-cases.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Update the properties of a cases object.|
|[Get ediscoveryCase](../api/ediscoverycase-get.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Read the properties and relationships of an [ediscoveryCase](../resources/ediscoverycase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|cases|[ediscoveryCase](../resources/ediscoverycase.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.compliance.ediscovery.contract.ediscovery",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.compliance.ediscovery.contract.ediscovery"
}
```

