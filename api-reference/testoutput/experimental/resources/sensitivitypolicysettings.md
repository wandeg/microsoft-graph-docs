---
title: "sensitivityPolicySettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# sensitivityPolicySettings resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sensitivityPolicySettingses](../api/sensitivitypolicysettings-list.md)|[sensitivityPolicySettings](../resources/sensitivityPolicySettings.md) collection|List properties and relationships of the [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) objects.|
|[Get sensitivityPolicySettings](../api/sensitivitypolicysettings-get.md)|[sensitivityPolicySettings](../resources/sensitivityPolicySettings.md)|Read properties and relationships of the [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.|
|[Create sensitivityPolicySettings](../api/sensitivitypolicysettings-create.md)|[sensitivityPolicySettings](../resources/sensitivityPolicySettings.md)|Create a new [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.|
|[Delete sensitivityPolicySettings](../api/sensitivitypolicysettings-delete.md)|None|Deletes a [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md).|
|[Update sensitivityPolicySettings](../api/sensitivitypolicysettings-update.md)|[sensitivityPolicySettings](../resources/sensitivityPolicySettings.md)|Update the properties of a [sensitivityPolicySettings](../resources/sensitivitypolicysettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|downgradeSensitivityRequiresJustification|Boolean||
|helpWebUrl|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isMandatory|Boolean||

## Relationships
None

## JSON Representation
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
  "downgradeSensitivityRequiresJustification": true
}
```

