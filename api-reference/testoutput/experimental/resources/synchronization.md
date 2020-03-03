---
title: "synchronization resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# synchronization resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List synchronizations](../api/synchronization-list.md)|[synchronization](../resources/synchronization.md) collection|List properties and relationships of the [synchronization](../resources/synchronization.md) objects.|
|[Get synchronization](../api/synchronization-get.md)|[synchronization](../resources/synchronization.md)|Read properties and relationships of the [synchronization](../resources/synchronization.md) object.|
|[Create synchronization](../api/synchronization-create.md)|[synchronization](../resources/synchronization.md)|Create a new [synchronization](../resources/synchronization.md) object.|
|[Delete synchronization](../api/synchronization-delete.md)|None|Deletes a [synchronization](../resources/synchronization.md).|
|[Update synchronization](../api/synchronization-update.md)|[synchronization](../resources/synchronization.md)|Update the properties of a [synchronization](../resources/synchronization.md) object.|
|[Ping](../api/synchronization-ping.md)|String||
|[List jobs](../api/synchronization-list-jobs.md)|[synchronizationJob](../resources/synchronizationJob.md) collection|Get the synchronizationJobs from the jobs navigation property.|
|[Add jobs](../api/synchronization-post-jobs.md)|[synchronizationJob](../resources/synchronizationJob.md)|Add jobs by posting to the jobs collection.|
|[List templates](../api/synchronization-list-templates.md)|[synchronizationTemplate](../resources/synchronizationTemplate.md) collection|Get the synchronizationTemplates from the templates navigation property.|
|[Add templates](../api/synchronization-post-templates.md)|[synchronizationTemplate](../resources/synchronizationTemplate.md)|Add templates by posting to the templates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|secrets|[synchronizationSecretKeyStringValuePair](../resources/synchronizationSecretKeyStringValuePair.md) collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|jobs|[synchronizationJob](../resources/synchronizationJob.md) collection||
|templates|[synchronizationTemplate](../resources/synchronizationTemplate.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronization",
  "id": "String (identifier)",
  "secrets": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair",
      "key": "String"
    }
  ]
}
```

