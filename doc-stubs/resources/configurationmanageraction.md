---
title: "configurationManagerAction resource type"
description: "Parameter for action triggerConfigurationManagerAction"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# configurationManagerAction resource type


Namespace: microsoft.graph

Parameter for action triggerConfigurationManagerAction

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|configurationManagerActionType|The action type to trigger on Configuration Manager client. Possible values are: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.configurationManagerAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.configurationManagerAction",
  "action": "String"
}
```

