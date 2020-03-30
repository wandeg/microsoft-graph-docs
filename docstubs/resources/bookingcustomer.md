---
title: "bookingCustomer resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bookingCustomer resource type


Namespace: microsoft.graph




Inherits from [bookingPerson](../resources/bookingperson.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get bookingCustomer](../api/bookingcustomer-get.md)|[bookingCustomer](../resources/bookingcustomer.md)|Read properties and relationships of the [bookingCustomer](../resources/bookingcustomer.md) object.|
|[Update bookingCustomer](../api/bookingcustomer-update.md)|[bookingCustomer](../resources/bookingcustomer.md)|Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String| Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String| Inherited from [bookingPerson](../resources/bookingperson.md)|
|id|String| Inherited from [entity](../resources/entity.md)|

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

