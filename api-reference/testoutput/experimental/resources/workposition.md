---
title: "workPosition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workPosition resource type


Namespace: microsoft.graph




Inherits from [itemFacet](../resources/itemfacet.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workPosition](../api/workposition-get.md)|[workPosition](../resources/workposition.md)|Read properties and relationships of the [workPosition](../resources/workposition.md) object.|
|[Update workPosition](../api/workposition-update.md)|[workPosition](../resources/workposition.md)|Update the properties of a [workPosition](../resources/workposition.md) object.|
|[List positions](../api/profile-list-positions.md)|[workPosition](../resources/workposition.md) collection|Get the workPositions from the positions navigation property.|
|[Add positions](../api/profile-post-positions.md)|[workPosition](../resources/workposition.md)|Add positions by posting to the positions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|String collection||
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|detail|[positionDetail](../resources/positiondetail.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workPosition",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workPosition",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "categories": [
    "String"
  ],
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail"
  }
}
```

