---
title: "shiftPreferences resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# shiftPreferences resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [changeTrackedEntity](../resources/changetrackedentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get shiftPreferences](../api/shiftpreferences-get.md)|[shiftPreferences](../resources/shiftpreferences.md)|Read the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.|
|[Update shiftPreferences](../api/shiftpreferences-update.md)|[shiftPreferences](../resources/shiftpreferences.md)|Update the properties of a [shiftPreferences](../resources/shiftpreferences.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availability|[shiftAvailability](../resources/shiftavailability.md) collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|

## Relationships
None

## JSON representation
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

