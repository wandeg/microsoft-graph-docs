---
title: "exactMatchLookupJob resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# exactMatchLookupJob resource type




Inherits from [exactMatchJobBase](../resources/exactMatchJobBase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List exactMatchLookupJobs](../api/exactmatchlookupjob-list.md)|[exactMatchLookupJob](../resources/exactMatchLookupJob.md) collection|List properties and relationships of the [exactMatchLookupJob](../resources/exactmatchlookupjob.md) objects.|
|[Get exactMatchLookupJob](../api/exactmatchlookupjob-get.md)|[exactMatchLookupJob](../resources/exactMatchLookupJob.md)|Read properties and relationships of the [exactMatchLookupJob](../resources/exactmatchlookupjob.md) object.|
|[Create exactMatchLookupJob](../api/exactmatchlookupjob-create.md)|[exactMatchLookupJob](../resources/exactMatchLookupJob.md)|Create a new [exactMatchLookupJob](../resources/exactmatchlookupjob.md) object.|
|[Delete exactMatchLookupJob](../api/exactmatchlookupjob-delete.md)|None|Deletes a [exactMatchLookupJob](../resources/exactmatchlookupjob.md).|
|[Update exactMatchLookupJob](../api/exactmatchlookupjob-update.md)|[exactMatchLookupJob](../resources/exactMatchLookupJob.md)|Update the properties of a [exactMatchLookupJob](../resources/exactmatchlookupjob.md) object.|
|[List matchingRows](../api/exactmatchlookupjob-list-matchingrows.md)|[lookupResultRow](../resources/lookupResultRow.md) collection|Get the lookupResultRows from the matchingRows navigation property.|
|[Add matchingRows](../api/exactmatchlookupjob-post-matchingrows.md)|[lookupResultRow](../resources/lookupResultRow.md)|Add matchingRows by posting to the matchingRows collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completionDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactMatchJobBase.md)|
|creationDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactMatchJobBase.md)|
|error|[classificationError](../resources/classificationError.md)| Inherited from [exactMatchJobBase](../resources/exactMatchJobBase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdatedDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactMatchJobBase.md)|
|startDateTime|DateTimeOffset| Inherited from [exactMatchJobBase](../resources/exactMatchJobBase.md)|
|state|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|matchingRows|[lookupResultRow](../resources/lookupResultRow.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.exactMatchLookupJob",
  "baseType": "microsoft.graph.exactMatchJobBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exactMatchLookupJob",
  "id": "String (identifier)",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.classificationError",
    "code": "String",
    "message": "String",
    "target": "String",
    "innerError": {
      "@odata.type": "microsoft.graph.classificationInnerError",
      "errorDateTime": "String (timestamp)",
      "clientRequestId": "String",
      "activityId": "String"
    },
    "details": [
      {
        "@odata.type": "microsoft.graph.classifcationErrorBase"
      }
    ]
  },
  "state": "String"
}
```

