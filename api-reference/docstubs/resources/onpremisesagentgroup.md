---
title: "onPremisesAgentGroup resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onPremisesAgentGroup resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onPremisesAgentGroup](../api/onpremisesagentgroup-get.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)|Read the properties and relationships of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.|
|[Update onPremisesAgentGroup](../api/onpremisesagentgroup-update.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)|Update the properties of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.|
|[List agents](../api/onpremisesagentgroup-list-agents.md)|[onPremisesAgent](../resources/onpremisesagent.md) collection|Get the onPremisesAgents from the agents navigation property.|
|[Add agents](../api/onpremisesagentgroup-post-agents.md)|[onPremisesAgent](../resources/onpremisesagent.md)|Add agents by posting to the agents collection.|
|[Remove agents](../api/onpremisesagentgroup-delete-agents.md)|None|Remove an [onPremisesAgent](../resources/onpremisesagent.md) object.|
|[List publishedResources](../api/onpremisesagentgroup-list-publishedresources.md)|[publishedResource](../resources/publishedresource.md) collection|Get the publishedResources from the publishedResources navigation property.|
|[Add publishedResources](../api/onpremisesagentgroup-post-publishedresources.md)|[publishedResource](../resources/publishedresource.md)|Add publishedResources by posting to the publishedResources collection.|
|[Remove publishedResources](../api/onpremisesagentgroup-delete-publishedresources.md)|None|Remove a [publishedResource](../resources/publishedresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean|**TODO: Add Description**|
|publishingType|onPremisesPublishingType|**TODO: Add Description**. Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|agents|[onPremisesAgent](../resources/onpremisesagent.md) collection|**TODO: Add Description**|
|publishedResources|[publishedResource](../resources/publishedresource.md) collection|**TODO: Add Description**|

## JSON representation
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

