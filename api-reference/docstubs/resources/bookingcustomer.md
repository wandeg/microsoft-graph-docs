---
title: "bookingCustomer resource type"
description: "Represents a customer of the business."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bookingCustomer resource type


Namespace: microsoft.graph

Represents a customer of the business.


Inherits from [bookingPerson](../resources/bookingperson.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get bookingCustomer](../api/bookingcustomer-get.md)|[bookingCustomer](../resources/bookingcustomer.md)|Read the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.|
|[Update bookingCustomer](../api/bookingcustomer-update.md)|[bookingCustomer](../resources/bookingcustomer.md)|Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String|The e-mail address of this person. Inherited from [bookingPerson](../resources/bookingperson.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCustomer",
  "baseType": "microsoft.graph.bookingPerson",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingCustomer",
  "id": "String (identifier)",
  "displayName": "String",
  "emailAddress": "String"
}
```

