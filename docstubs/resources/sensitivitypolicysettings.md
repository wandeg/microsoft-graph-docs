---
title: "sensitivityPolicySettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sensitivityPolicySettings resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get sensitivityPolicySettings](../api/sensitivitypolicysettings-get.md)|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md)|Read properties and relationships of the [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.|
|[Update sensitivityPolicySettings](../api/sensitivitypolicysettings-update.md)|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md)|Update the properties of a [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicableTo|Enumeration| Possible values are: `email`, `site`, `unifiedGroup`, `unknownFutureValue`.|
|downgradeSensitivityRequiresJustification|Boolean||
|helpWebUrl|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isMandatory|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sensitivityPolicySettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sensitivityPolicySettings",
  "id": "String (identifier)",
  "isMandatory": true,
  "helpWebUrl": "String",
  "downgradeSensitivityRequiresJustification": true,
  "applicableTo": "String"
}
```

