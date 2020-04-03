---
title: "synchronization resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# synchronization resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get synchronization](../api/synchronization-get.md)|[synchronization](../resources/synchronization.md)|Read properties and relationships of the [synchronization](../resources/synchronization.md) object.|
|[Update synchronization](../api/synchronization-update.md)|[synchronization](../resources/synchronization.md)|Update the properties of a [synchronization](../resources/synchronization.md) object.|
|[Ping](../api/synchronization-ping.md)|String||
|[List jobs](../api/synchronization-list-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md) collection|Get the synchronizationJobs from the jobs navigation property.|
|[Add jobs](../api/synchronization-post-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md)|Add jobs by posting to the jobs collection.|
|[List templates](../api/synchronization-list-templates.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md) collection|Get the synchronizationTemplates from the templates navigation property.|
|[Add templates](../api/synchronization-post-templates.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Add templates by posting to the templates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|secrets|[synchronizationSecretKeyStringValuePair](../resources/synchronizationsecretkeystringvaluepair.md) collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|jobs|[synchronizationJob](../resources/synchronizationjob.md) collection||
|templates|[synchronizationTemplate](../resources/synchronizationtemplate.md) collection||

## JSON representation
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

