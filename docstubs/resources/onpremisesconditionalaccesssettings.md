---
title: "onPremisesConditionalAccessSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onPremisesConditionalAccessSettings resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|
|[Update onPremisesConditionalAccessSettings](../api/onpremisesconditionalaccesssettings-update.md)|[onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md)|Update the properties of a [onPremisesConditionalAccessSettings](../resources/onpremisesconditionalaccesssettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|enabled|Boolean||
|excludedGroups|Guid collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|includedGroups|Guid collection||
|overrideDefaultRule|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```

