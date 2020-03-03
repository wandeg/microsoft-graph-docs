---
title: "messageRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# messageRule resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get messageRule](../api/messagerule-get.md)|[messageRule](../resources/messageRule.md)|Read properties and relationships of the [messageRule](../resources/messagerule.md) object.|
|[Delete messageRule](../api/messagerule-delete.md)|None|Deletes a [messageRule](../resources/messagerule.md).|
|[Update messageRule](../api/messagerule-update.md)|[messageRule](../resources/messageRule.md)|Update the properties of a [messageRule](../resources/messagerule.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actions|[messageRuleActions](../resources/messageRuleActions.md)||
|conditions|[messageRulePredicates](../resources/messageRulePredicates.md)||
|displayName|String||
|exceptions|[messageRulePredicates](../resources/messageRulePredicates.md)||
|hasError|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|isEnabled|Boolean||
|isReadOnly|Boolean||
|sequence|Int32||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.messageRule",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.messageRule",
  "id": "String (identifier)",
  "displayName": "String",
  "sequence": 1024,
  "conditions": {
    "@odata.type": "microsoft.graph.messageRulePredicates"
  },
  "actions": {
    "@odata.type": "microsoft.graph.messageRuleActions"
  },
  "exceptions": {
    "@odata.type": "microsoft.graph.messageRulePredicates"
  },
  "isEnabled": true,
  "hasError": true,
  "isReadOnly": true
}
```

