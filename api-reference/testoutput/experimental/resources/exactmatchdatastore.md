---
title: "exactMatchDataStore resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# exactMatchDataStore resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get exactMatchDataStore](../api/exactmatchdatastore-get.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md)|Read properties and relationships of the [exactMatchDataStore](../resources/exactmatchdatastore.md) object.|
|[Update exactMatchDataStore](../api/exactmatchdatastore-update.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md)|Update the properties of a [exactMatchDataStore](../resources/exactmatchdatastore.md) object.|
|[lookup](../api/exactmatchdatastore-lookup.md)|String collection||
|[List sessions](../api/exactmatchdatastore-list-sessions.md)|[exactMatchSession](../resources/exactmatchsession.md) collection|Get the exactMatchSessions from the sessions navigation property.|
|[Add sessions](../api/exactmatchdatastore-post-sessions.md)|[exactMatchSession](../resources/exactmatchsession.md)|Add sessions by posting to the sessions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|dataLastUpdatedDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sessions|[exactMatchSession](../resources/exactmatchsession.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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

