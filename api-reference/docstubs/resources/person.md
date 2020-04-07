---
title: "person resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# person resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get person](../api/person-get.md)|[person](../resources/person.md)|Read properties and relationships of the [person](../resources/person.md) object.|
|[Update person](../api/person-update.md)|[person](../resources/person.md)|Update the properties of a [person](../resources/person.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|birthday|String||
|companyName|String||
|department|String||
|displayName|String||
|emailAddresses|[rankedEmailAddress](../resources/rankedemailaddress.md) collection||
|givenName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isFavorite|Boolean||
|mailboxType|String||
|officeLocation|String||
|personNotes|String||
|personType|String||
|phones|[phone](../resources/phone.md) collection||
|postalAddresses|[location](../resources/location.md) collection||
|profession|String||
|sources|[personDataSource](../resources/persondatasource.md) collection||
|surname|String||
|title|String||
|userPrincipalName|String||
|websites|[website](../resources/website.md) collection||
|yomiCompany|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.person",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.person",
  "id": "String (identifier)",
  "displayName": "String",
  "givenName": "String",
  "surname": "String",
  "birthday": "String",
  "personNotes": "String",
  "isFavorite": true,
  "emailAddresses": [
    {
      "@odata.type": "microsoft.graph.rankedEmailAddress"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ],
  "postalAddresses": [
    {
      "@odata.type": "microsoft.graph.location"
    }
  ],
  "websites": [
    {
      "@odata.type": "microsoft.graph.website"
    }
  ],
  "title": "String",
  "companyName": "String",
  "yomiCompany": "String",
  "department": "String",
  "officeLocation": "String",
  "profession": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.personDataSource"
    }
  ],
  "mailboxType": "String",
  "personType": "String",
  "userPrincipalName": "String"
}
```

