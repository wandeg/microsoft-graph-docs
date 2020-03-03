---
title: "educationSynchronizationError resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationSynchronizationError resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List educationSynchronizationErrors](../api/educationsynchronizationerror-list.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md) collection|List properties and relationships of the [educationSynchronizationError](../resources/educationsynchronizationerror.md) objects.|
|[Get educationSynchronizationError](../api/educationsynchronizationerror-get.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md)|Read properties and relationships of the [educationSynchronizationError](../resources/educationsynchronizationerror.md) object.|
|[Create educationSynchronizationError](../api/educationsynchronizationerror-create.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md)|Create a new [educationSynchronizationError](../resources/educationsynchronizationerror.md) object.|
|[Delete educationSynchronizationError](../api/educationsynchronizationerror-delete.md)|None|Deletes a [educationSynchronizationError](../resources/educationsynchronizationerror.md).|
|[Update educationSynchronizationError](../api/educationsynchronizationerror-update.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md)|Update the properties of a [educationSynchronizationError](../resources/educationsynchronizationerror.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|entryType|String||
|errorCode|String||
|errorMessage|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|joiningValue|String||
|recordedDateTime|DateTimeOffset||
|reportableIdentifier|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationSynchronizationError",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationError",
  "id": "String (identifier)",
  "entryType": "String",
  "errorCode": "String",
  "errorMessage": "String",
  "joiningValue": "String",
  "recordedDateTime": "String (timestamp)",
  "reportableIdentifier": "String"
}
```

