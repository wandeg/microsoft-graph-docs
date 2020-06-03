---
title: "cloudCommunications resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# cloudCommunications resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List cloudCommunications](../api/cloudcommunications-list.md)|[cloudCommunications](../resources/cloudcommunications.md) collection|Get a list of the [cloudCommunications](../resources/cloudcommunications.md) objects and their properties.|
|[Create cloudCommunications](../api/cloudcommunications-create.md)|[cloudCommunications](../resources/cloudcommunications.md)|Create a new [cloudCommunications](../resources/cloudcommunications.md) object.|
|[Get cloudCommunications](../api/cloudcommunications-get.md)|[cloudCommunications](../resources/cloudcommunications.md)|Read the properties and relationships of a [cloudCommunications](../resources/cloudcommunications.md) object.|
|[Update cloudCommunications](../api/cloudcommunications-update.md)|[cloudCommunications](../resources/cloudcommunications.md)|Update the properties of a [cloudCommunications](../resources/cloudcommunications.md) object.|
|[Delete cloudCommunications](../api/cloudcommunications-delete.md)|None|Deletes a [cloudCommunications](../resources/cloudcommunications.md) object.|
|[List presences](../api/cloudcommunications-list-presences.md)|[presence](../resources/presence.md) collection|Get the presences from the presences navigation property.|
|[Create presences](../api/cloudcommunications-post-presences.md)|[presence](../resources/presence.md)|Create a new presences object.|
|[Get presences](../api/cloudcommunications-get-presence.md)|[presence](../resources/presence.md)|Read the properties and relationships of a [presence](../resources/presence.md) object.|
|[Update presences](../api/cloudcommunications-update-presences.md)|[presence](../resources/presence.md)|Update the properties of a presences object.|
|[Delete presences](../api/cloudcommunications-delete-presences.md)|None|Delete a [presence](../resources/presence.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|callRecords|[callRecord](../resources/callrecord.md) collection|**TODO: Add Description**|
|calls|[call](../resources/call.md) collection|**TODO: Add Description**|
|onlineMeetings|[onlineMeeting](../resources/onlinemeeting.md) collection|**TODO: Add Description**|
|presences|[presence](../resources/presence.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudCommunications",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudCommunications",
  "id": "String (identifier)"
}
```

