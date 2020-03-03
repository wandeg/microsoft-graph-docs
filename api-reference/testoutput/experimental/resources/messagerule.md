---
title: "messageRule resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# messageRule resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List messageRules](../api/messagerule-list.md)|[messageRule](../resources/messagerule.md) collection|List properties and relationships of the [messageRule](../resources/messagerule.md) objects.|
|[Get messageRule](../api/messagerule-get.md)|[messageRule](../resources/messagerule.md)|Read properties and relationships of the [messageRule](../resources/messagerule.md) object.|
|[Create messageRule](../api/messagerule-create.md)|[messageRule](../resources/messagerule.md)|Create a new [messageRule](../resources/messagerule.md) object.|
|[Delete messageRule](../api/messagerule-delete.md)|None|Deletes a [messageRule](../resources/messagerule.md).|
|[Update messageRule](../api/messagerule-update.md)|[messageRule](../resources/messagerule.md)|Update the properties of a [messageRule](../resources/messagerule.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actions|[messageRuleActions](../resources/messageruleactions.md)||
|conditions|[messageRulePredicates](../resources/messagerulepredicates.md)||
|displayName|String||
|exceptions|[messageRulePredicates](../resources/messagerulepredicates.md)||
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

