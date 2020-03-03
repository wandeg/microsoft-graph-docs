---
title: "changeTrackedEntity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# changeTrackedEntity resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List changeTrackedEntities](../api/changetrackedentity-list.md)|[changeTrackedEntity](../resources/changetrackedentity.md) collection|List properties and relationships of the [changeTrackedEntity](../resources/changetrackedentity.md) objects.|
|[Get changeTrackedEntity](../api/changetrackedentity-get.md)|[changeTrackedEntity](../resources/changetrackedentity.md)|Read properties and relationships of the [changeTrackedEntity](../resources/changetrackedentity.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)||
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.changeTrackedEntity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.changeTrackedEntity",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

