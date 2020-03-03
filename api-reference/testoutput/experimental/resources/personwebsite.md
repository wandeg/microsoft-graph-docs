---
title: "personWebsite resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# personWebsite resource type




Inherits from [itemFacet](../resources/itemFacet.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get personWebsite](../api/personwebsite-get.md)|[personWebsite](../resources/personWebsite.md)|Read properties and relationships of the [personWebsite](../resources/personwebsite.md) object.|
|[Delete personWebsite](../api/personwebsite-delete.md)|None|Deletes a [personWebsite](../resources/personwebsite.md).|
|[Update personWebsite](../api/personwebsite-update.md)|[personWebsite](../resources/personWebsite.md)|Update the properties of a [personWebsite](../resources/personwebsite.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemFacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|String collection||
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemFacet.md)|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|inference|[inferenceData](../resources/inferenceData.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [itemFacet](../resources/itemFacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemFacet.md)|
|webUrl|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personWebsite",
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
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```

