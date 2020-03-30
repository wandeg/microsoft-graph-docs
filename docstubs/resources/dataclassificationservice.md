---
title: "dataClassificationService resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# dataClassificationService resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get dataClassificationService](../api/dataclassificationservice-get.md)|[dataClassificationService](../resources/dataclassificationservice.md)|Read properties and relationships of the [dataClassificationService](../resources/dataclassificationservice.md) object.|
|[Update dataClassificationService](../api/dataclassificationservice-update.md)|[dataClassificationService](../resources/dataclassificationservice.md)|Update the properties of a [dataClassificationService](../resources/dataclassificationservice.md) object.|
|[List exactMatchDataStores](../api/dataclassificationservice-list-exactmatchdatastores.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md) collection|Get the exactMatchDataStores from the exactMatchDataStores navigation property.|
|[Add exactMatchDataStores](../api/dataclassificationservice-post-exactmatchdatastores.md)|[exactMatchDataStore](../resources/exactmatchdatastore.md)|Add exactMatchDataStores by posting to the exactMatchDataStores collection.|
|[List sensitiveTypes](../api/dataclassificationservice-list-sensitivetypes.md)|[sensitiveType](../resources/sensitivetype.md) collection|Get the sensitiveTypes from the sensitiveTypes navigation property.|
|[Add sensitiveTypes](../api/dataclassificationservice-post-sensitivetypes.md)|[sensitiveType](../resources/sensitivetype.md)|Add sensitiveTypes by posting to the sensitiveTypes collection.|
|[List jobs](../api/dataclassificationservice-list-jobs.md)|[jobResponseBase](../resources/jobresponsebase.md) collection|Get the jobResponseBases from the jobs navigation property.|
|[Add jobs](../api/dataclassificationservice-post-jobs.md)|[jobResponseBase](../resources/jobresponsebase.md)|Add jobs by posting to the jobs collection.|
|[List classifyFileJobs](../api/dataclassificationservice-list-classifyfilejobs.md)|[jobResponseBase](../resources/jobresponsebase.md) collection|Get the jobResponseBases from the classifyFileJobs navigation property.|
|[Add classifyFileJobs](../api/dataclassificationservice-post-classifyfilejobs.md)|[jobResponseBase](../resources/jobresponsebase.md)|Add classifyFileJobs by posting to the classifyFileJobs collection.|
|[List classifyTextJobs](../api/dataclassificationservice-list-classifytextjobs.md)|[jobResponseBase](../resources/jobresponsebase.md) collection|Get the jobResponseBases from the classifyTextJobs navigation property.|
|[Add classifyTextJobs](../api/dataclassificationservice-post-classifytextjobs.md)|[jobResponseBase](../resources/jobresponsebase.md)|Add classifyTextJobs by posting to the classifyTextJobs collection.|
|[List evaluateLabelJobs](../api/dataclassificationservice-list-evaluatelabeljobs.md)|[jobResponseBase](../resources/jobresponsebase.md) collection|Get the jobResponseBases from the evaluateLabelJobs navigation property.|
|[Add evaluateLabelJobs](../api/dataclassificationservice-post-evaluatelabeljobs.md)|[jobResponseBase](../resources/jobresponsebase.md)|Add evaluateLabelJobs by posting to the evaluateLabelJobs collection.|
|[List evaluateDlpPoliciesJobs](../api/dataclassificationservice-list-evaluatedlppoliciesjobs.md)|[jobResponseBase](../resources/jobresponsebase.md) collection|Get the jobResponseBases from the evaluateDlpPoliciesJobs navigation property.|
|[Add evaluateDlpPoliciesJobs](../api/dataclassificationservice-post-evaluatedlppoliciesjobs.md)|[jobResponseBase](../resources/jobresponsebase.md)|Add evaluateDlpPoliciesJobs by posting to the evaluateDlpPoliciesJobs collection.|
|[List labelsAndPoliciesEvaluationJobs](../api/dataclassificationservice-list-labelsandpoliciesevaluationjobs.md)|[jobResponseBase](../resources/jobresponsebase.md) collection|Get the jobResponseBases from the labelsAndPoliciesEvaluationJobs navigation property.|
|[Add labelsAndPoliciesEvaluationJobs](../api/dataclassificationservice-post-labelsandpoliciesevaluationjobs.md)|[jobResponseBase](../resources/jobresponsebase.md)|Add labelsAndPoliciesEvaluationJobs by posting to the labelsAndPoliciesEvaluationJobs collection.|
|[List classifyText](../api/dataclassificationservice-list-classifytext.md)|[textClassificationRequest](../resources/textclassificationrequest.md) collection|Get the textClassificationRequests from the classifyText navigation property.|
|[Add classifyText](../api/dataclassificationservice-post-classifytext.md)|[textClassificationRequest](../resources/textclassificationrequest.md)|Add classifyText by posting to the classifyText collection.|
|[List classifyFile](../api/dataclassificationservice-list-classifyfile.md)|[fileClassificationRequest](../resources/fileclassificationrequest.md) collection|Get the fileClassificationRequests from the classifyFile navigation property.|
|[Add classifyFile](../api/dataclassificationservice-post-classifyfile.md)|[fileClassificationRequest](../resources/fileclassificationrequest.md)|Add classifyFile by posting to the classifyFile collection.|
|[List sensitivityLabels](../api/dataclassificationservice-list-sensitivitylabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md) collection|Get the sensitivityLabels from the sensitivityLabels navigation property.|
|[Add sensitivityLabels](../api/dataclassificationservice-post-sensitivitylabels.md)|[sensitivityLabel](../resources/sensitivitylabel.md)|Add sensitivityLabels by posting to the sensitivityLabels collection.|
|[List exactMatchUploadAgents](../api/dataclassificationservice-list-exactmatchuploadagents.md)|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md) collection|Get the exactMatchUploadAgents from the exactMatchUploadAgents navigation property.|
|[Add exactMatchUploadAgents](../api/dataclassificationservice-post-exactmatchuploadagents.md)|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md)|Add exactMatchUploadAgents by posting to the exactMatchUploadAgents collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|classifyFile|[fileClassificationRequest](../resources/fileclassificationrequest.md) collection||
|classifyFileJobs|[jobResponseBase](../resources/jobresponsebase.md) collection||
|classifyText|[textClassificationRequest](../resources/textclassificationrequest.md) collection||
|classifyTextJobs|[jobResponseBase](../resources/jobresponsebase.md) collection||
|evaluateDlpPoliciesJobs|[jobResponseBase](../resources/jobresponsebase.md) collection||
|evaluateLabelJobs|[jobResponseBase](../resources/jobresponsebase.md) collection||
|exactMatchDataStores|[exactMatchDataStore](../resources/exactmatchdatastore.md) collection||
|exactMatchUploadAgents|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md) collection||
|jobs|[jobResponseBase](../resources/jobresponsebase.md) collection||
|labelsAndPoliciesEvaluationJobs|[jobResponseBase](../resources/jobresponsebase.md) collection||
|sensitiveTypes|[sensitiveType](../resources/sensitivetype.md) collection||
|sensitivityLabels|[sensitivityLabel](../resources/sensitivitylabel.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataClassificationService",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataClassificationService",
  "id": "String (identifier)"
}
```

