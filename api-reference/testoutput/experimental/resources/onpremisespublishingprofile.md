---
title: "onPremisesPublishingProfile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# onPremisesPublishingProfile resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List onPremisesPublishingProfiles](../api/onpremisespublishingprofile-list.md)|[onPremisesPublishingProfile](../resources/onPremisesPublishingProfile.md) collection|List properties and relationships of the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) objects.|
|[Get onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md)|[onPremisesPublishingProfile](../resources/onPremisesPublishingProfile.md)|Read properties and relationships of the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.|
|[Create onPremisesPublishingProfile](../api/onpremisespublishingprofile-post-onpremisespublishingprofiles.md)|[onPremisesPublishingProfile](../resources/onPremisesPublishingProfile.md)|Create a new [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.|
|[Delete onPremisesPublishingProfile](../api/onpremisespublishingprofile-delete.md)|None|Deletes a [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md).|
|[Update onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md)|[onPremisesPublishingProfile](../resources/onPremisesPublishingProfile.md)|Update the properties of a [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.|
|[List agents](../api/onpremisespublishingprofile-list-agents.md)|[onPremisesAgent](../resources/onPremisesAgent.md) collection|Get the onPremisesAgents from the agents navigation property.|
|[Add agents](../api/onpremisespublishingprofile-post-agents.md)|[onPremisesAgent](../resources/onPremisesAgent.md)|Add agents by posting to the agents collection.|
|[List agentGroups](../api/onpremisespublishingprofile-list-agentgroups.md)|[onPremisesAgentGroup](../resources/onPremisesAgentGroup.md) collection|Get the onPremisesAgentGroups from the agentGroups navigation property.|
|[Add agentGroups](../api/onpremisespublishingprofile-post-agentgroups.md)|[onPremisesAgentGroup](../resources/onPremisesAgentGroup.md)|Add agentGroups by posting to the agentGroups collection.|
|[List publishedResources](../api/onpremisespublishingprofile-list-publishedresources.md)|[publishedResource](../resources/publishedResource.md) collection|Get the publishedResources from the publishedResources navigation property.|
|[Add publishedResources](../api/onpremisespublishingprofile-post-publishedresources.md)|[publishedResource](../resources/publishedResource.md)|Add publishedResources by posting to the publishedResources collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](../resources/hybridAgentUpdaterConfiguration.md)||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|agentGroups|[onPremisesAgentGroup](../resources/onPremisesAgentGroup.md) collection||
|agents|[onPremisesAgent](../resources/onPremisesAgent.md) collection||
|publishedResources|[publishedResource](../resources/publishedResource.md) collection||

## JSON Representation
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

