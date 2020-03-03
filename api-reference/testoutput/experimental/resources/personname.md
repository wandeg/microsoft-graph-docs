---
title: "personName resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# personName resource type




Inherits from [itemFacet](../resources/itemFacet.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get personName](../api/personname-get.md)|[personName](../resources/personName.md)|Read properties and relationships of the [personName](../resources/personname.md) object.|
|[Delete personName](../api/personname-delete.md)|None|Deletes a [personName](../resources/personname.md).|
|[Update personName](../api/personname-update.md)|[personName](../resources/personName.md)|Update the properties of a [personName](../resources/personname.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemFacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemFacet.md)|
|displayName|String||
|first|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|inference|[inferenceData](../resources/inferenceData.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|initials|String||
|languageTag|String||
|last|String||
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemFacet.md)|
|maiden|String||
|middle|String||
|nickname|String||
|pronunciation|[yomiPersonName](../resources/yomiPersonName.md)||
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

