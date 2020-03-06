---
title: "personAnniversary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# personAnniversary resource type


Namespace: microsoft.graph




Inherits from [itemFacet](../resources/itemfacet.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get personAnniversary](../api/personanniversary-get.md)|[personAnniversary](../resources/personanniversary.md)|Read properties and relationships of the [personAnniversary](../resources/personanniversary.md) object.|
|[Update personAnniversary](../api/personanniversary-update.md)|[personAnniversary](../resources/personanniversary.md)|Update the properties of a [personAnniversary](../resources/personanniversary.md) object.|
|[List anniversaries](../api/profile-list-anniversaries.md)|[personAnniversary](../resources/personanniversary.md) collection|Get the personAnniversaries from the anniversaries navigation property.|
|[Add anniversaries](../api/profile-post-anniversaries.md)|[personAnniversary](../resources/personanniversary.md)|Add anniversaries by posting to the anniversaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|date|Date||
|id|String| Inherited from [entity](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|type|Enumeration|. Possible values are: `birthday`, `wedding`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAnniversary",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAnniversary",
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
  "type": "String",
  "date": "Date"
}
```

