---
title: "evaluateLabelsAndPoliciesJobResponse resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# evaluateLabelsAndPoliciesJobResponse resource type


Namespace: microsoft.graph




Inherits from [jobResponseBase](../resources/jobresponsebase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List evaluateLabelsAndPoliciesJobResponses](../api/evaluatelabelsandpoliciesjobresponse-list.md)|[evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md) collection|List properties and relationships of the [evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md) objects.|
|[Get evaluateLabelsAndPoliciesJobResponse](../api/evaluatelabelsandpoliciesjobresponse-get.md)|[evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md)|Read properties and relationships of the [evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md) object.|
|[Create evaluateLabelsAndPoliciesJobResponse](../api/evaluatelabelsandpoliciesjobresponse-create.md)|[evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md)|Create a new [evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md) object.|
|[Delete evaluateLabelsAndPoliciesJobResponse](../api/evaluatelabelsandpoliciesjobresponse-delete.md)|None|Deletes a [evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md).|
|[Update evaluateLabelsAndPoliciesJobResponse](../api/evaluatelabelsandpoliciesjobresponse-update.md)|[evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md)|Update the properties of a [evaluateLabelsAndPoliciesJobResponse](../resources/evaluatelabelsandpoliciesjobresponse.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|endDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|error|[classificationError](../resources/classificationerror.md)| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|result|[evaluateLabelsAndPoliciesResult](../resources/evaluatelabelsandpoliciesresult.md)||
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
  "@odata.type": "microsoft.graph.evaluateLabelsAndPoliciesJobResponse",
  "baseType": "microsoft.graph.jobResponseBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.evaluateLabelsAndPoliciesJobResponse",
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
    "@odata.type": "microsoft.graph.evaluateLabelsAndPoliciesResult"
  }
}
```

