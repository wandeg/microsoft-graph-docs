---
title: "exactMatchDataStore resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# exactMatchDataStore resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[lookup](../api/exactmatchdatastore-lookup.md)|String collection|**TODO: Add Description**|
|[List sessions](../api/exactmatchdatastore-list-sessions.md)|[exactMatchSession](../resources/exactmatchsession.md) collection|Get the exactMatchSessions from the sessions navigation property.|
|[Create sessions](../api/exactmatchdatastore-post-sessions.md)|[exactMatchSession](../resources/exactmatchsession.md)|Create a new sessions object.|
|[Delete sessions](../api/exactmatchdatastore-delete-sessions.md)|None|Delete a [exactMatchSession](../resources/exactmatchsession.md) object.|
|[Update sessions](../api/exactmatchdatastore-update-sessions.md)|[exactMatchSession](../resources/exactmatchsession.md)|Update the properties of a sessions object.|
|[Get exactMatchSession](../api/exactmatchsession-get.md)|[exactMatchSession](../resources/exactmatchsession.md)|Read the properties and relationships of an [exactMatchSession](../resources/exactmatchsession.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|dataLastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sessions|[exactMatchSession](../resources/exactmatchsession.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.exactMatchDataStore",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exactMatchDataStore",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "dataLastUpdatedDateTime": "String (timestamp)"
}
```

