---
title: "educationSynchronizationError resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationSynchronizationError resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationSynchronizationError](../api/educationsynchronizationerror-get.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md)|Read the properties and relationships of an [educationSynchronizationError](../resources/educationsynchronizationerror.md) object.|
|[Update educationSynchronizationError](../api/educationsynchronizationerror-update.md)|[educationSynchronizationError](../resources/educationsynchronizationerror.md)|Update the properties of an [educationSynchronizationError](../resources/educationsynchronizationerror.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|entryType|String|**TODO: Add Description**|
|errorCode|String|**TODO: Add Description**|
|errorMessage|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|joiningValue|String|**TODO: Add Description**|
|recordedDateTime|DateTimeOffset|**TODO: Add Description**|
|reportableIdentifier|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

