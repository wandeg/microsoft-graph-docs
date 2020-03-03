---
title: "personName resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# personName resource type


Namespace: microsoft.graph




Inherits from [itemFacet](../resources/itemfacet.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List personNames](../api/personname-list.md)|[personName](../resources/personname.md) collection|List properties and relationships of the [personName](../resources/personname.md) objects.|
|[Get personName](../api/personname-get.md)|[personName](../resources/personname.md)|Read properties and relationships of the [personName](../resources/personname.md) object.|
|[Create personName](../api/personname-create.md)|[personName](../resources/personname.md)|Create a new [personName](../resources/personname.md) object.|
|[Delete personName](../api/personname-delete.md)|None|Deletes a [personName](../resources/personname.md).|
|[Update personName](../api/personname-update.md)|[personName](../resources/personname.md)|Update the properties of a [personName](../resources/personname.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|displayName|String||
|first|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|initials|String||
|languageTag|String||
|last|String||
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|maiden|String||
|middle|String||
|nickname|String||
|pronunciation|[yomiPersonName](../resources/yomipersonname.md)||
|suffix|String||
|title|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personName",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personName",
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
  "displayName": "String",
  "first": "String",
  "initials": "String",
  "last": "String",
  "languageTag": "String",
  "maiden": "String",
  "middle": "String",
  "nickname": "String",
  "suffix": "String",
  "title": "String",
  "pronunciation": {
    "@odata.type": "microsoft.graph.yomiPersonName"
  }
}
```

