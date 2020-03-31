---
title: "cartToClassAssociation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# cartToClassAssociation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get cartToClassAssociation](../api/carttoclassassociation-get.md)|[cartToClassAssociation](../resources/carttoclassassociation.md)|Read properties and relationships of the [cartToClassAssociation](../resources/carttoclassassociation.md) object.|
|[Update cartToClassAssociation](../api/carttoclassassociation-update.md)|[cartToClassAssociation](../resources/carttoclassassociation.md)|Update the properties of a [cartToClassAssociation](../resources/carttoclassassociation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classroomIds|String collection||
|createdDateTime|DateTimeOffset||
|description|String||
|deviceCartIds|String collection||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|version|Int32||

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

