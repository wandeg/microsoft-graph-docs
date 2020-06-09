---
title: "conditionalAccessRoot resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# conditionalAccessRoot resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List conditionalAccessRoots](../api/conditionalaccessroot-list.md)|[conditionalAccessRoot](../resources/conditionalaccessroot.md) collection|Get a list of the [conditionalAccessRoot](../resources/conditionalaccessroot.md) objects and their properties.|
|[Create conditionalAccessRoot](../api/conditionalaccessroot-create.md)|[conditionalAccessRoot](../resources/conditionalaccessroot.md)|Create a new [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.|
|[Get conditionalAccessRoot](../api/conditionalaccessroot-get.md)|[conditionalAccessRoot](../resources/conditionalaccessroot.md)|Read the properties and relationships of a [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.|
|[Update conditionalAccessRoot](../api/conditionalaccessroot-update.md)|[conditionalAccessRoot](../resources/conditionalaccessroot.md)|Update the properties of a [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.|
|[Delete conditionalAccessRoot](../api/conditionalaccessroot-delete.md)|None|Deletes a [conditionalAccessRoot](../resources/conditionalaccessroot.md) object.|
|[List namedLocations](../api/conditionalaccessroot-list-namedlocations.md)|[namedLocation](../resources/namedlocation.md) collection|Get the namedLocations from the namedLocations navigation property.|
|[Create namedLocations](../api/conditionalaccessroot-post-namedlocations.md)|[namedLocation](../resources/namedlocation.md)|Create a new namedLocations object.|
|[Get namedLocations](../api/conditionalaccessroot-get-namedlocation.md)|[namedLocation](../resources/namedlocation.md)|Read the properties and relationships of a [namedLocation](../resources/namedlocation.md) object.|
|[Update namedLocations](../api/conditionalaccessroot-update-namedlocations.md)|[namedLocation](../resources/namedlocation.md)|Update the properties of a namedLocations object.|
|[Delete namedLocations](../api/conditionalaccessroot-delete-namedlocations.md)|None|Delete a [namedLocation](../resources/namedlocation.md) object.|
|[List policies](../api/conditionalaccessroot-list-policies.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) collection|Get the conditionalAccessPolicies from the policies navigation property.|
|[Create policies](../api/conditionalaccessroot-post-policies.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Create a new policies object.|
|[Get policies](../api/conditionalaccessroot-get-conditionalaccesspolicy.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Read the properties and relationships of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|
|[Update policies](../api/conditionalaccessroot-update-policies.md)|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)|Update the properties of a policies object.|
|[Delete policies](../api/conditionalaccessroot-delete-policies.md)|None|Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|namedLocations|[namedLocation](../resources/namedlocation.md) collection|**TODO: Add Description**|
|policies|[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conditionalAccessRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessRoot",
  "id": "String (identifier)"
}
```

