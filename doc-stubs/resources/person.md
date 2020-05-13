---
title: "person resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# person resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|birthday|String|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|imAddress|String|**TODO: Add Description**|
|isFavorite|Boolean|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|personNotes|String|**TODO: Add Description**|
|personType|[personType](../resources/persontype.md)|**TODO: Add Description**|
|phones|[phone](../resources/phone.md) collection|**TODO: Add Description**|
|postalAddresses|[location](../resources/location.md) collection|**TODO: Add Description**|
|profession|String|**TODO: Add Description**|
|scoredEmailAddresses|[scoredEmailAddress](../resources/scoredemailaddress.md) collection|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|websites|[website](../resources/website.md) collection|**TODO: Add Description**|
|yomiCompany|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "isFavorite": "Boolean",
  "scoredEmailAddresses": [
    {
      "@odata.type": "microsoft.graph.scoredEmailAddress"
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
  "jobTitle": "String",
  "companyName": "String",
  "yomiCompany": "String",
  "department": "String",
  "officeLocation": "String",
  "profession": "String",
  "personType": {
    "@odata.type": "microsoft.graph.personType"
  },
  "userPrincipalName": "String",
  "imAddress": "String"
}
```

