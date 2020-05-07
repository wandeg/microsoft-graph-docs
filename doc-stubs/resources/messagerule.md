---
title: "messageRule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# messageRule resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actions|[messageRuleActions](../resources/messageruleactions.md)|**TODO: Add Description**|
|conditions|[messageRulePredicates](../resources/messagerulepredicates.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|exceptions|[messageRulePredicates](../resources/messagerulepredicates.md)|**TODO: Add Description**|
|hasError|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isEnabled|Boolean|**TODO: Add Description**|
|isReadOnly|Boolean|**TODO: Add Description**|
|sequence|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "sequence": "Integer",
  "conditions": {
    "@odata.type": "microsoft.graph.messageRulePredicates"
  },
  "actions": {
    "@odata.type": "microsoft.graph.messageRuleActions"
  },
  "exceptions": {
    "@odata.type": "microsoft.graph.messageRulePredicates"
  },
  "isEnabled": "Boolean",
  "hasError": "Boolean",
  "isReadOnly": "Boolean"
}
```

