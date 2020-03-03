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
|[List exactMatchDataStores](../api/exactmatchdatastore-list.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md) collection|List properties and relationships of the [exactMatchDataStore](../resources/exactmatchdatastore.md) objects.|
|[Get exactMatchDataStore](../api/exactmatchdatastore-get.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md)|Read properties and relationships of the [exactMatchDataStore](../resources/exactmatchdatastore.md) object.|
|[Create exactMatchDataStore](../api/exactmatchdatastore-create.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md)|Create a new [exactMatchDataStore](../resources/exactmatchdatastore.md) object.|
|[Delete exactMatchDataStore](../api/exactmatchdatastore-delete.md)|None|Deletes a [exactMatchDataStore](../resources/exactmatchdatastore.md).|
|[Update exactMatchDataStore](../api/exactmatchdatastore-update.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md)|Update the properties of a [exactMatchDataStore](../resources/exactmatchdatastore.md) object.|
|[lookup](../api/exactmatchdatastore-lookup.md)|String collection||
|[List sessions](../api/exactmatchdatastore-list-sessions.md)|[exactMatchSession](../resources/exactmatchsession.md) collection|Get the exactMatchSessions from the sessions navigation property.|
|[Add sessions](../api/exactmatchdatastore-post-sessions.md)|[exactMatchSession](../resources/exactmatchsession.md)|Add sessions by posting to the sessions collection.|
|[List exactMatchDataStores](../api/dataclassificationservice-list-exactmatchdatastores.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md) collection|Get the exactMatchDataStores from the exactMatchDataStores navigation property.|
|[Add exactMatchDataStores](../api/dataclassificationservice-post-exactmatchdatastores.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md)|Add exactMatchDataStores by posting to the exactMatchDataStores collection.|

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

## JSON Representation
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

