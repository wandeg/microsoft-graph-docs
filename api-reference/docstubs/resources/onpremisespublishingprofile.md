---
title: "onPremisesPublishingProfile resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onPremisesPublishingProfile resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List onPremisesPublishingProfiles](../api/onpremisespublishingprofile-list.md)|[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) collection|Get a list of the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) objects and their properties.|
|[Get onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md)|[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)|Read the properties and relationships of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.|
|[Create onPremisesPublishingProfile](../api/onpremisespublishingprofile-post-onpremisespublishingprofiles.md)|[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)|Create a new [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.|
|[Delete onPremisesPublishingProfile](../api/onpremisespublishingprofile-delete.md)|None|Deletes an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.|
|[Update onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md)|[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)|Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.|
|[List agents](../api/onpremisespublishingprofile-list-agents.md)|[onPremisesAgent](../resources/onpremisesagent.md) collection|Get the onPremisesAgents from the agents navigation property.|
|[Create agents](../api/onpremisespublishingprofile-post-agents.md)|[onPremisesAgent](../resources/onpremisesagent.md)|Create a new agents object.|
|[Delete agents](../api/onpremisespublishingprofile-delete-agents.md)|None|Delete an [onPremisesAgent](../resources/onpremisesagent.md) object.|
|[Update agents](../api/onpremisespublishingprofile-update-agents.md)|[onPremisesAgent](../resources/onpremisesagent.md)|Update the properties of an agents object.|
|[Get onPremisesAgent](../api/onpremisesagent-get.md)|[onPremisesAgent](../resources/onpremisesagent.md)|Read the properties and relationships of an [onPremisesAgent](../resources/onpremisesagent.md) object.|
|[List agentGroups](../api/onpremisespublishingprofile-list-agentgroups.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md) collection|Get the onPremisesAgentGroups from the agentGroups navigation property.|
|[Create agentGroups](../api/onpremisespublishingprofile-post-agentgroups.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)|Create a new agentGroups object.|
|[Delete agentGroups](../api/onpremisespublishingprofile-delete-agentgroups.md)|None|Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.|
|[Update agentGroups](../api/onpremisespublishingprofile-update-agentgroups.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)|Update the properties of an agentGroups object.|
|[Get onPremisesAgentGroup](../api/onpremisesagentgroup-get.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)|Read the properties and relationships of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.|
|[List publishedResources](../api/onpremisespublishingprofile-list-publishedresources.md)|[publishedResource](../resources/publishedresource.md) collection|Get the publishedResources from the publishedResources navigation property.|
|[Create publishedResources](../api/onpremisespublishingprofile-post-publishedresources.md)|[publishedResource](../resources/publishedresource.md)|Create a new publishedResources object.|
|[Delete publishedResources](../api/onpremisespublishingprofile-delete-publishedresources.md)|None|Delete a [publishedResource](../resources/publishedresource.md) object.|
|[Update publishedResources](../api/onpremisespublishingprofile-update-publishedresources.md)|[publishedResource](../resources/publishedresource.md)|Update the properties of a publishedResources object.|
|[Get publishedResource](../api/publishedresource-get.md)|[publishedResource](../resources/publishedresource.md)|Read the properties and relationships of a [publishedResource](../resources/publishedresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|agentGroups|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md) collection|**TODO: Add Description**|
|agents|[onPremisesAgent](../resources/onpremisesagent.md) collection|**TODO: Add Description**|
|publishedResources|[publishedResource](../resources/publishedresource.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesPublishingProfile",
  "id": "String (identifier)",
  "hybridAgentUpdaterConfiguration": {
    "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
    "deferUpdateDateTime": "String (timestamp)",
    "updateWindow": {
      "@odata.type": "microsoft.graph.updateWindow",
      "updateWindowStartTime": "String (time of day)",
      "updateWindowEndTime": "String (time of day)"
    },
    "allowUpdateConfigurationOverride": true
  }
}
```

