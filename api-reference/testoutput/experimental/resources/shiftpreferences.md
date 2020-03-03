---
title: "shiftPreferences resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# shiftPreferences resource type


Namespace: microsoft.graph




Inherits from [changeTrackedEntity](../resources/changetrackedentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List shiftPreferenceses](../api/shiftpreferences-list.md)|[shiftPreferences](../resources/shiftpreferences.md) collection|List properties and relationships of the [shiftPreferences](../resources/shiftpreferences.md) objects.|
|[Get shiftPreferences](../api/shiftpreferences-get.md)|[shiftPreferences](../resources/shiftpreferences.md)|Read properties and relationships of the [shiftPreferences](../resources/shiftpreferences.md) object.|
|[Create shiftPreferences](../api/shiftpreferences-create.md)|[shiftPreferences](../resources/shiftpreferences.md)|Create a new [shiftPreferences](../resources/shiftpreferences.md) object.|
|[Delete shiftPreferences](../api/shiftpreferences-delete.md)|None|Deletes a [shiftPreferences](../resources/shiftpreferences.md).|
|[Update shiftPreferences](../api/shiftpreferences-update.md)|[shiftPreferences](../resources/shiftpreferences.md)|Update the properties of a [shiftPreferences](../resources/shiftpreferences.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availability|[shiftAvailability](../resources/shiftavailability.md) collection||
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|

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

