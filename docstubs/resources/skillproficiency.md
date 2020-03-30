---
title: "skillProficiency resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# skillProficiency resource type


Namespace: microsoft.graph




Inherits from [itemFacet](../resources/itemfacet.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get skillProficiency](../api/skillproficiency-get.md)|[skillProficiency](../resources/skillproficiency.md)|Read properties and relationships of the [skillProficiency](../resources/skillproficiency.md) object.|
|[Update skillProficiency](../api/skillproficiency-update.md)|[skillProficiency](../resources/skillproficiency.md)|Update the properties of a [skillProficiency](../resources/skillproficiency.md) object.|
|[List skills](../api/profile-list-skills.md)|[skillProficiency](../resources/skillproficiency.md) collection|Get the skillProficiencies from the skills navigation property.|
|[Add skills](../api/profile-post-skills.md)|[skillProficiency](../resources/skillproficiency.md)|Add skills by posting to the skills collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|String collection||
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|proficiency|Enumeration| Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.|
|webUrl|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skillProficiency",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skillProficiency",
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
  "displayName": "String",
  "proficiency": "String",
  "webUrl": "String"
}
```

