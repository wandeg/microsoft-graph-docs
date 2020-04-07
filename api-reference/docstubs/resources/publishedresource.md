---
title: "publishedResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# publishedResource resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get publishedResource](../api/publishedresource-get.md)|[publishedResource](../resources/publishedresource.md)|Read properties and relationships of the [publishedResource](../resources/publishedresource.md) object.|
|[Update publishedResource](../api/publishedresource-update.md)|[publishedResource](../resources/publishedresource.md)|Update the properties of a [publishedResource](../resources/publishedresource.md) object.|
|[List agentGroups](../api/publishedresource-list-agentgroups.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md) collection|Get the onPremisesAgentGroups from the agentGroups navigation property.|
|[Create agentGroups](../api/publishedresource-post-agentgroups.md)|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)|Create agentGroups by posting to the agentGroups collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|publishingType|Enumeration| Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `intunePfx`, `oflineDomainJoin`, `unknownFutureValue`.|
|resourceName|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|agentGroups|[onPremisesAgentGroup](../resources/onpremisesagentgroup.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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

