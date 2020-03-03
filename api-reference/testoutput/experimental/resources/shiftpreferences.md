---
title: "shiftPreferences resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# shiftPreferences resource type




Inherits from [changeTrackedEntity](../resources/changeTrackedEntity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List shiftPreferenceses](../api/shiftpreferences-list.md)|[shiftPreferences](../resources/shiftPreferences.md) collection|List properties and relationships of the [shiftPreferences](../resources/shiftpreferences.md) objects.|
|[Get shiftPreferences](../api/shiftpreferences-get.md)|[shiftPreferences](../resources/shiftPreferences.md)|Read properties and relationships of the [shiftPreferences](../resources/shiftpreferences.md) object.|
|[Create shiftPreferences](../api/shiftpreferences-create.md)|[shiftPreferences](../resources/shiftPreferences.md)|Create a new [shiftPreferences](../resources/shiftpreferences.md) object.|
|[Delete shiftPreferences](../api/shiftpreferences-delete.md)|None|Deletes a [shiftPreferences](../resources/shiftpreferences.md).|
|[Update shiftPreferences](../api/shiftpreferences-update.md)|[shiftPreferences](../resources/shiftPreferences.md)|Update the properties of a [shiftPreferences](../resources/shiftpreferences.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availability|[shiftAvailability](../resources/shiftAvailability.md) collection||
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftPreferences",
  "baseType": "microsoft.graph.changeTrackedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.shiftPreferences",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "availability": [
    {
      "@odata.type": "microsoft.graph.shiftAvailability"
    }
  ]
}
```

