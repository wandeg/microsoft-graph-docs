---
title: "onPremisesAgent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onPremisesAgent resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List agentGroups](../api/onpremisesagent-list-agentgroups.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md) collection|Get the onPremisesAgentGroups from the agentGroups navigation property.|
|[Add agentGroups](../api/onpremisesagent-post-agentgroups.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)|Add agentGroups by posting to the agentGroups collection.|
|[Remove agentGroups](../api/onpremisesagent-delete-agentgroups.md)|None|Remove an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.|
|[List agents](../api/onpremisesagentgroup-list-agents.md)|[onPremisesAgent](../resources/onpremisesagent.md) collection|Get the onPremisesAgents from the agents navigation property.|
|[Add agents](../api/onpremisesagentgroup-post-agents.md)|[onPremisesAgent](../resources/onpremisesagent.md)|Add agents by posting to the agents collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|externalIp|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|machineName|String|**TODO: Add Description**|
|status|agentStatus|**TODO: Add Description**. Possible values are: `active`, `inactive`.|
|supportedPublishingTypes|onPremisesPublishingType collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|agentGroups|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesAgent",
  "id": "String (identifier)",
  "machineName": "String",
  "externalIp": "String",
  "status": "String",
  "supportedPublishingTypes": [
    "String"
  ]
}
```

