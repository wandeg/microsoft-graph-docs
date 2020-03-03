---
title: "onPremisesAgent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# onPremisesAgent resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List onPremisesAgents](../api/onpremisesagent-list.md)|[onPremisesAgent](../resources/onPremisesAgent.md) collection|List properties and relationships of the [onPremisesAgent](../resources/onpremisesagent.md) objects.|
|[Get onPremisesAgent](../api/onpremisesagent-get.md)|[onPremisesAgent](../resources/onPremisesAgent.md)|Read properties and relationships of the [onPremisesAgent](../resources/onpremisesagent.md) object.|
|[Create onPremisesAgent](../api/onpremisesagent-create.md)|[onPremisesAgent](../resources/onPremisesAgent.md)|Create a new [onPremisesAgent](../resources/onpremisesagent.md) object.|
|[Delete onPremisesAgent](../api/onpremisesagent-delete.md)|None|Deletes a [onPremisesAgent](../resources/onpremisesagent.md).|
|[Update onPremisesAgent](../api/onpremisesagent-update.md)|[onPremisesAgent](../resources/onPremisesAgent.md)|Update the properties of a [onPremisesAgent](../resources/onpremisesagent.md) object.|
|[List agentGroups](../api/onpremisesagent-list-agentgroups.md)|[onPremisesAgentGroup](../resources/onPremisesAgentGroup.md) collection|Get the onPremisesAgentGroups from the agentGroups navigation property.|
|[Create agentGroups](../api/onpremisesagent-post-agentgroups.md)|[onPremisesAgentGroup](../resources/onPremisesAgentGroup.md)|Create agentGroups by posting to the agentGroups collection.|

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
|agentGroups|[onPremisesAgentGroup](../resources/onPremisesAgentGroup.md) collection||

## JSON Representation
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

