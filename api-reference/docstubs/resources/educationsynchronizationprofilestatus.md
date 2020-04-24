---
title: "educationSynchronizationProfileStatus resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationSynchronizationProfileStatus resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationSynchronizationProfileStatus](../api/educationsynchronizationprofilestatus-get.md)|[educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md)|Read the properties and relationships of an [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.|
|[Update educationSynchronizationProfileStatus](../api/educationsynchronizationprofilestatus-update.md)|[educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md)|Update the properties of an [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSynchronizationDateTime|DateTimeOffset|**TODO: Add Description**|
|status|educationSynchronizationStatus|**TODO: Add Description**. Possible values are: `paused`, `inProgress`, `success`, `error`, `validationError`, `quarantined`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
  "id": "String (identifier)",
  "status": "String",
  "lastSynchronizationDateTime": "String (timestamp)"
}
```

