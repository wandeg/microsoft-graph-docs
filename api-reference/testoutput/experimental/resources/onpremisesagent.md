---
title: "onPremisesAgent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onPremisesAgent resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onPremisesAgent](../api/onpremisesagent-get.md)|[onPremisesAgent](../resources/onpremisesagent.md)|Read properties and relationships of the [onPremisesAgent](../resources/onpremisesagent.md) object.|
|[Update onPremisesAgent](../api/onpremisesagent-update.md)|[onPremisesAgent](../resources/onpremisesagent.md)|Update the properties of a [onPremisesAgent](../resources/onpremisesagent.md) object.|
|[List agentGroups](../api/onpremisesagent-list-agentgroups.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md) collection|Get the onPremisesAgentGroups from the agentGroups navigation property.|
|[Create agentGroups](../api/onpremisesagent-post-agentgroups.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)|Create agentGroups by posting to the agentGroups collection.|
|[List agents](../api/onpremisesagentgroup-list-agents.md)|[onPremisesAgent](../resources/onpremisesagent.md) collection|Get the onPremisesAgents from the agents navigation property.|
|[Create agents](../api/onpremisesagentgroup-post-agents.md)|[onPremisesAgent](../resources/onpremisesagent.md)|Create agents by posting to the agents collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|externalIp|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|machineName|String||
|status|Enumeration|. Possible values are: `active`, `inactive`.|
|supportedPublishingTypes|Enumeration collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|agentGroups|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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

