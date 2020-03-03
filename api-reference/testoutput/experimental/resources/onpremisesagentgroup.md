---
title: "onPremisesAgentGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# onPremisesAgentGroup resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onPremisesAgentGroup](../api/onpremisesagentgroup-get.md)|[onPremisesAgentGroup](../resources/onPremisesAgentGroup.md)|Read properties and relationships of the [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.|
|[Delete onPremisesAgentGroup](../api/onpremisesagentgroup-delete.md)|None|Deletes a [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).|
|[Update onPremisesAgentGroup](../api/onpremisesagentgroup-update.md)|[onPremisesAgentGroup](../resources/onPremisesAgentGroup.md)|Update the properties of a [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.|
|[List agents](../api/onpremisesagentgroup-list-agents.md)|[onPremisesAgent](../resources/onPremisesAgent.md) collection|Get the onPremisesAgents from the agents navigation property.|
|[Create agents](../api/onpremisesagentgroup-post-agents.md)|[onPremisesAgent](../resources/onPremisesAgent.md)|Create agents by posting to the agents collection.|
|[List publishedResources](../api/onpremisesagentgroup-list-publishedresources.md)|[publishedResource](../resources/publishedResource.md) collection|Get the publishedResources from the publishedResources navigation property.|
|[Create publishedResources](../api/onpremisesagentgroup-post-publishedresources.md)|[publishedResource](../resources/publishedResource.md)|Create publishedResources by posting to the publishedResources collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean||
|publishingType|Enumeration|. Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|agents|[onPremisesAgent](../resources/onPremisesAgent.md) collection||
|publishedResources|[publishedResource](../resources/publishedResource.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesAgentGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "publishingType": "String",
  "isDefault": true
}
```

