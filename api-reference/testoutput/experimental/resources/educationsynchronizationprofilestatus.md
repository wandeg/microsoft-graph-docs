---
title: "educationSynchronizationProfileStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationSynchronizationProfileStatus resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationSynchronizationProfileStatus](../api/educationsynchronizationprofilestatus-get.md)|[educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md)|Read properties and relationships of the [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.|
|[Update educationSynchronizationProfileStatus](../api/educationsynchronizationprofilestatus-update.md)|[educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md)|Update the properties of a [educationSynchronizationProfileStatus](../resources/educationsynchronizationprofilestatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSynchronizationDateTime|DateTimeOffset||
|status|Enumeration|. Possible values are: `paused`, `inProgress`, `success`, `error`, `validationError`, `quarantined`, `unknownFutureValue`.|

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

