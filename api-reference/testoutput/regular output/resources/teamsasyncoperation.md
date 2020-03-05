---
title: "teamsAsyncOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsAsyncOperation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List teamsAsyncOperations](../api/teamsasyncoperation-list.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md) collection|List properties and relationships of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) objects.|
|[Get teamsAsyncOperation](../api/teamsasyncoperation-get.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Read properties and relationships of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.|
|[Create teamsAsyncOperation](../api/teamsasyncoperation-create.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Create a new [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.|
|[Delete teamsAsyncOperation](../api/teamsasyncoperation-delete.md)|None|Deletes a [teamsAsyncOperation](../resources/teamsasyncoperation.md).|
|[Update teamsAsyncOperation](../api/teamsasyncoperation-update.md)|[teamsAsyncOperation](../resources/teamsasyncoperation.md)|Update the properties of a [teamsAsyncOperation](../resources/teamsasyncoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attemptsCount|Int32||
|createdDateTime|DateTimeOffset||
|error|[operationError](../resources/operationerror.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastActionDateTime|DateTimeOffset||
|operationType|Enumeration|. Possible values are: `invalid`, `cloneTeam`, `archiveTeam`, `unarchiveTeam`, `createTeam`, `unknownFutureValue`.|
|status|Enumeration|. Possible values are: `invalid`, `notStarted`, `inProgress`, `succeeded`, `failed`, `unknownFutureValue`.|
|targetResourceId|String||
|targetResourceLocation|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAsyncOperation",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAsyncOperation",
  "id": "String (identifier)",
  "operationType": "String",
  "createdDateTime": "String (timestamp)",
  "status": "String",
  "lastActionDateTime": "String (timestamp)",
  "attemptsCount": 1024,
  "targetResourceId": "String",
  "targetResourceLocation": "String",
  "error": {
    "@odata.type": "microsoft.graph.operationError"
  }
}
```

