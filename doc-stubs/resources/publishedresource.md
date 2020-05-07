---
title: "publishedResource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# publishedResource resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List agentGroups](../api/publishedresource-list-agentgroups.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md) collection|Get the onPremisesAgentGroups from the agentGroups navigation property.|
|[Add agentGroups](../api/publishedresource-post-agentgroups.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)|Add agentGroups by posting to the agentGroups collection.|
|[Remove agentGroups](../api/publishedresource-delete-agentgroups.md)|None|Remove an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.|
|[List publishedResources](../api/onpremisesagentgroup-list-publishedresources.md)|[publishedResource](../resources/publishedresource.md) collection|Get the publishedResources from the publishedResources navigation property.|
|[Add publishedResources](../api/onpremisesagentgroup-post-publishedresources.md)|[publishedResource](../resources/publishedresource.md)|Add publishedResources by posting to the publishedResources collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|publishingType|onPremisesPublishingType|**TODO: Add Description**. Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|
|resourceName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|agentGroups|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.publishedResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publishedResource",
  "id": "String (identifier)",
  "displayName": "String",
  "resourceName": "String",
  "publishingType": "String"
}
```

