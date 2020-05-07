---
title: "synchronizationJob resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationJob resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[pause](../api/synchronizationjob-pause.md)|None|**TODO: Add Description**|
|[start](../api/synchronizationjob-start.md)|None|**TODO: Add Description**|
|[stop](../api/synchronizationjob-stop.md)|None|**TODO: Add Description**|
|[apply](../api/synchronizationjob-apply.md)|None|**TODO: Add Description**|
|[restart](../api/synchronizationjob-restart.md)|None|**TODO: Add Description**|
|[validateCredentials](../api/synchronizationjob-validatecredentials.md)|None|**TODO: Add Description**|
|[validateCredentials](../api/synchronizationjob-validatecredentials.md)|None|**TODO: Add Description**|
|[List schema](../api/synchronizationjob-list-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md) collection|Get the synchronizationSchemas from the schema navigation property.|
|[Create schema](../api/synchronizationjob-post-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Create a new schema object.|
|[Delete schema](../api/synchronizationjob-delete-schema.md)|None|Delete a [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[Update schema](../api/synchronizationjob-update-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Update the properties of a schema object.|
|[Get synchronizationSchema](../api/synchronizationschema-get.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Read the properties and relationships of a [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[List jobs](../api/synchronization-list-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md) collection|Get the synchronizationJobs from the jobs navigation property.|
|[Create jobs](../api/synchronization-post-jobs.md)|[synchronizationJob](../resources/synchronizationjob.md)|Create a new jobs object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|schedule|[synchronizationSchedule](../resources/synchronizationschedule.md)|**TODO: Add Description**|
|status|[synchronizationStatus](../resources/synchronizationstatus.md)|**TODO: Add Description**|
|synchronizationJobSettings|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|schema|[synchronizationSchema](../resources/synchronizationschema.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationJob",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJob",
  "id": "String (identifier)",
  "templateId": "String",
  "schedule": {
    "@odata.type": "microsoft.graph.synchronizationSchedule"
  },
  "status": {
    "@odata.type": "microsoft.graph.synchronizationStatus"
  },
  "synchronizationJobSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```

