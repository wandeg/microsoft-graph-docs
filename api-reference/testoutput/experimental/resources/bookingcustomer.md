---
title: "bookingCustomer resource type"
description: "Represents a customer of the business."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# bookingCustomer resource type

Represents a customer of the business.


Inherits from [bookingPerson](../resources/bookingPerson.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get bookingCustomer](../api/bookingcustomer-get.md)|[bookingCustomer](../resources/bookingCustomer.md)|Read properties and relationships of the [bookingCustomer](../resources/bookingcustomer.md) object.|
|[Delete bookingCustomer](../api/bookingcustomer-delete.md)|None|Deletes a [bookingCustomer](../resources/bookingcustomer.md).|
|[Update bookingCustomer](../api/bookingcustomer-update.md)|[bookingCustomer](../resources/bookingCustomer.md)|Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.|
|[List customers](../api/bookingbusiness-list-customers.md)|[bookingCustomer](../resources/bookingCustomer.md) collection|Get the bookingCustomers from the customers navigation property.|
|[Add customers](../api/bookingbusiness-post-customers.md)|[bookingCustomer](../resources/bookingCustomer.md)|Add customers by posting to the customers collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingNamedEntity.md)|
|emailAddress|String|The e-mail address of this person. Inherited from [bookingPerson](../resources/bookingPerson.md)|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
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

