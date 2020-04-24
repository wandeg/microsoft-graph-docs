---
title: "sensitivityPolicySettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# sensitivityPolicySettings resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get sensitivityPolicySettings](../api/sensitivitypolicysettings-get.md)|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md)|Read the properties and relationships of a [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.|
|[Update sensitivityPolicySettings](../api/sensitivitypolicysettings-update.md)|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md)|Update the properties of a [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.|
|[List sensitivityPolicySettings](../api/informationprotection-list-sensitivitypolicysettings.md)|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) collection|Get the sensitivityPolicySettings from the sensitivityPolicySettings navigation property.|
|[Create sensitivityPolicySettings](../api/informationprotection-post-sensitivitypolicysettings.md)|[sensitivityPolicySettings](../resources/sensitivitypolicysettings.md)|Create a new sensitivityPolicySettings object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicableTo|sensitivityLabelTarget|**TODO: Add Description**. Possible values are: `email`, `site`, `unifiedGroup`, `unknownFutureValue`.|
|downgradeSensitivityRequiresJustification|Boolean|**TODO: Add Description**|
|helpWebUrl|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isMandatory|Boolean|**TODO: Add Description**|

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

