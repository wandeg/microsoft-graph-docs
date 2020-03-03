---
title: "evaluateLabelJobResponse resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# evaluateLabelJobResponse resource type


Namespace: microsoft.graph




Inherits from [jobResponseBase](../resources/jobresponsebase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List evaluateLabelJobResponses](../api/evaluatelabeljobresponse-list.md)|[evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) collection|List properties and relationships of the [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) objects.|
|[Get evaluateLabelJobResponse](../api/evaluatelabeljobresponse-get.md)|[evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md)|Read properties and relationships of the [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) object.|
|[Create evaluateLabelJobResponse](../api/evaluatelabeljobresponse-create.md)|[evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md)|Create a new [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) object.|
|[Delete evaluateLabelJobResponse](../api/evaluatelabeljobresponse-delete.md)|None|Deletes a [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md).|
|[Update evaluateLabelJobResponse](../api/evaluatelabeljobresponse-update.md)|[evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md)|Update the properties of a [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|endDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|error|[classificationError](../resources/classificationerror.md)| Inherited from [jobResponseBase](../resources/jobresponsebase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|result|[evaluateLabelJobResultGroup](../resources/evaluatelabeljobresultgroup.md)||
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
  "@odata.type": "microsoft.graph.evaluateLabelJobResponse",
  "baseType": "microsoft.graph.jobResponseBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.evaluateLabelJobResponse",
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
    "@odata.type": "microsoft.graph.evaluateLabelJobResultGroup"
  }
}
```

