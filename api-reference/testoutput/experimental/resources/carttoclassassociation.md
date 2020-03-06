---
title: "cartToClassAssociation resource type"
description: "CartToClassAssociation for associating device carts with classrooms."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# cartToClassAssociation resource type


Namespace: microsoft.graph

CartToClassAssociation for associating device carts with classrooms.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get cartToClassAssociation](../api/carttoclassassociation-get.md)|[cartToClassAssociation](../resources/carttoclassassociation.md)|Read properties and relationships of the [cartToClassAssociation](../resources/carttoclassassociation.md) object.|
|[Update cartToClassAssociation](../api/carttoclassassociation-update.md)|[cartToClassAssociation](../resources/carttoclassassociation.md)|Update the properties of a [cartToClassAssociation](../resources/carttoclassassociation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classroomIds|String collection|Identifiers of classrooms to be associated with device carts.|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the CartToClassAssociation.|
|deviceCartIds|String collection|Identifiers of device carts to be associated with classes.|
|displayName|String|Admin provided name of the device configuration.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|version|Int32|Version of the CartToClassAssociation.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cartToClassAssociation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "classroomIds": [
    "String"
  ]
}
```

