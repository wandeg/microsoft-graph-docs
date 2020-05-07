---
title: "bookingCustomer resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bookingCustomer resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [bookingPerson](../resources/bookingperson.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String|**TODO: Add Description** Inherited from [bookingPerson](../resources/bookingperson.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

