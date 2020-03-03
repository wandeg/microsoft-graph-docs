---
title: "dlpEvaluatePoliciesJobResponse resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# dlpEvaluatePoliciesJobResponse resource type


Namespace: microsoft.graph




Inherits from [jobResponseBase](../resources/jobresponsebase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List dlpEvaluatePoliciesJobResponses](../api/dlpevaluatepoliciesjobresponse-list.md)|[dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md) collection|List properties and relationships of the [dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md) objects.|
|[Get dlpEvaluatePoliciesJobResponse](../api/dlpevaluatepoliciesjobresponse-get.md)|[dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md)|Read properties and relationships of the [dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md) object.|
|[Create dlpEvaluatePoliciesJobResponse](../api/dlpevaluatepoliciesjobresponse-create.md)|[dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md)|Create a new [dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md) object.|
|[Delete dlpEvaluatePoliciesJobResponse](../api/dlpevaluatepoliciesjobresponse-delete.md)|None|Deletes a [dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md).|
|[Update dlpEvaluatePoliciesJobResponse](../api/dlpevaluatepoliciesjobresponse-update.md)|[dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md)|Update the properties of a [dlpEvaluatePoliciesJobResponse](../resources/dlpevaluatepoliciesjobresponse.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|endDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|error|[classificationError](../resources/classificationerror.md)| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|result|[dlpPoliciesJobResult](../resources/dlppoliciesjobresult.md)||
|startDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|status|String| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|tenantId|String| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|type|String| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dlpEvaluatePoliciesJobResponse",
  "baseType": "microsoft.graph.jobResponseBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dlpEvaluatePoliciesJobResponse",
  "id": "String (identifier)",
  "type": "String",
  "status": "String",
  "tenantId": "String",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.classificationError"
  },
  "result": {
    "@odata.type": "microsoft.graph.dlpPoliciesJobResult"
  }
}
```

