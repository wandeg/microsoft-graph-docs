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


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List onPremisesPublishingProfiles](../api/onpremisespublishingprofile-list.md)|[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) collection|Get a list of the [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) objects and their properties.|
|[Create onPremisesPublishingProfile](../api/onpremisespublishingprofile-post-onpremisespublishingprofiles.md)|[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)|Create a new [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.|
|[Get onPremisesPublishingProfile](../api/onpremisespublishingprofile-get.md)|[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)|Read the properties and relationships of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.|
|[Update onPremisesPublishingProfile](../api/onpremisespublishingprofile-update.md)|[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)|Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.|
|[Delete onPremisesPublishingProfile](../api/onpremisespublishingprofile-delete.md)|None|Deletes an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.|
|[List connectorGroups](../api/onpremisespublishingprofile-list-connectorgroups.md)|[connectorGroup](../resources/connectorgroup.md) collection|Get the connectorGroups from the connectorGroups navigation property.|
|[Create connectorGroups](../api/onpremisespublishingprofile-post-connectorgroups.md)|[connectorGroup](../resources/connectorgroup.md)|Create a new connectorGroups object.|
|[Get connectorGroups](../api/onpremisespublishingprofile-get-connectorgroup.md)|[connectorGroup](../resources/connectorgroup.md)|Read the properties and relationships of a [connectorGroup](../resources/connectorgroup.md) object.|
|[Update connectorGroups](../api/onpremisespublishingprofile-update-connectorgroups.md)|[connectorGroup](../resources/connectorgroup.md)|Update the properties of a connectorGroups object.|
|[Delete connectorGroups](../api/onpremisespublishingprofile-delete-connectorgroups.md)|None|Delete a [connectorGroup](../resources/connectorgroup.md) object.|
|[List connectors](../api/onpremisespublishingprofile-list-connectors.md)|[connector](../resources/connector.md) collection|Get the connectors from the connectors navigation property.|
|[Create connectors](../api/onpremisespublishingprofile-post-connectors.md)|[connector](../resources/connector.md)|Create a new connectors object.|
|[Get connectors](../api/onpremisespublishingprofile-get-connector.md)|[connector](../resources/connector.md)|Read the properties and relationships of a [connector](../resources/connector.md) object.|
|[Update connectors](../api/onpremisespublishingprofile-update-connectors.md)|[connector](../resources/connector.md)|Update the properties of a connectors object.|
|[Delete connectors](../api/onpremisespublishingprofile-delete-connectors.md)|None|Delete a [connector](../resources/connector.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|hybridAgentUpdaterConfiguration|[hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isEnabled|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|agentGroups|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md) collection|**TODO: Add Description**|
|agents|[onPremisesAgent](../resources/onpremisesagent.md) collection|**TODO: Add Description**|
|connectorGroups|[connectorGroup](../resources/connectorgroup.md) collection|**TODO: Add Description**|
|connectors|[connector](../resources/connector.md) collection|**TODO: Add Description**|
|publishedResources|[publishedResource](../resources/publishedresource.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "isEnabled": "Boolean",
  "hybridAgentUpdaterConfiguration": {
    "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"
  }
}
```

