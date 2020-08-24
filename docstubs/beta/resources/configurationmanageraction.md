---
title: "configurationManagerAction resource type"
description: "Parameter for action triggerConfigurationManagerAction"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# configurationManagerAction resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Parameter for action triggerConfigurationManagerAction

## Properties

| Property | Type   | Description                                                |
| :------- | :----- | :--------------------------------------------------------- |
| action   | String | The action type to trigger on Configuration Manager client |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerAction",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.configurationManagerAction",
  "action": "refreshMachinePolicy | refreshUserPolicy | wakeUpClient | appEvaluation"
}
```