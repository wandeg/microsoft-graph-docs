---
title: "synchronization resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronization resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Ping](../api/synchronization-ping.md)|String|**TODO: Add Description**|
|[List jobs](../api/synchronization-list-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md) collection|Get the synchronizationJobs from the jobs navigation property.|
|[Create jobs](../api/synchronization-post-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md)|Create a new jobs object.|
|[Delete jobs](../api/synchronization-delete-jobs.md)|None|Delete a [synchronizationJob](../resources/synchronizationjob.md) object.|
|[Update jobs](../api/synchronization-update-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md)|Update the properties of a jobs object.|
|[Get synchronizationJob](../api/synchronizationjob-get.md)|[synchronizationJob](../resources/synchronizationjob.md)|Read the properties and relationships of a [synchronizationJob](../resources/synchronizationjob.md) object.|
|[List templates](../api/synchronization-list-templates.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md) collection|Get the synchronizationTemplates from the templates navigation property.|
|[Create templates](../api/synchronization-post-templates.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Create a new templates object.|
|[Delete templates](../api/synchronization-delete-templates.md)|None|Delete a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Update templates](../api/synchronization-update-templates.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Update the properties of a templates object.|
|[Get synchronizationTemplate](../api/synchronizationtemplate-get.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Read the properties and relationships of a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[List synchronization](../api/application-list-synchronization.md)|[synchronization](../resources/synchronization.md) collection|Get the synchronizations from the synchronization navigation property.|
|[Create synchronization](../api/application-post-synchronization.md)|[synchronization](../resources/synchronization.md)|Create a new synchronization object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|secrets|[synchronizationSecretKeyStringValuePair](../resources/synchronizationsecretkeystringvaluepair.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|jobs|[synchronizationJob](../resources/synchronizationjob.md) collection|**TODO: Add Description**|
|templates|[synchronizationTemplate](../resources/synchronizationtemplate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```

