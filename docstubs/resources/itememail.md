---
title: "itemEmail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# itemEmail resource type


Namespace: microsoft.graph




Inherits from [itemFacet](../resources/itemfacet.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get itemEmail](../api/itememail-get.md)|[itemEmail](../resources/itememail.md)|Read properties and relationships of the [itemEmail](../resources/itememail.md) object.|
|[Update itemEmail](../api/itememail-update.md)|[itemEmail](../resources/itememail.md)|Update the properties of a [itemEmail](../resources/itememail.md) object.|
|[List emails](../api/profile-list-emails.md)|[itemEmail](../resources/itememail.md) collection|Get the itemEmails from the emails navigation property.|
|[Add emails](../api/profile-post-emails.md)|[itemEmail](../resources/itememail.md)|Add emails by posting to the emails collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|String||
|allowedAudiences|Enumeration| Inherited from [itemFacet](../resources/itemfacet.md). Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|createdDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|inference|[inferenceData](../resources/inferencedata.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [itemFacet](../resources/itemfacet.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [itemFacet](../resources/itemfacet.md)|
|type|Enumeration| Possible values are: `unknown`, `work`, `personal`, `main`, `other`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemEmail",
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
  "address": "String",
  "displayName": "String",
  "type": "String"
}
```

