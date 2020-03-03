---
title: "evaluateLabelJobResponse resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# evaluateLabelJobResponse resource type




Inherits from [jobResponseBase](../resources/jobResponseBase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List evaluateLabelJobResponses](../api/evaluatelabeljobresponse-list.md)|[evaluateLabelJobResponse](../resources/evaluateLabelJobResponse.md) collection|List properties and relationships of the [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) objects.|
|[Get evaluateLabelJobResponse](../api/evaluatelabeljobresponse-get.md)|[evaluateLabelJobResponse](../resources/evaluateLabelJobResponse.md)|Read properties and relationships of the [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) object.|
|[Create evaluateLabelJobResponse](../api/evaluatelabeljobresponse-create.md)|[evaluateLabelJobResponse](../resources/evaluateLabelJobResponse.md)|Create a new [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) object.|
|[Delete evaluateLabelJobResponse](../api/evaluatelabeljobresponse-delete.md)|None|Deletes a [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md).|
|[Update evaluateLabelJobResponse](../api/evaluatelabeljobresponse-update.md)|[evaluateLabelJobResponse](../resources/evaluateLabelJobResponse.md)|Update the properties of a [evaluateLabelJobResponse](../resources/evaluatelabeljobresponse.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|endDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|error|[classificationError](../resources/classificationError.md)| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|result|[evaluateLabelJobResultGroup](../resources/evaluateLabelJobResultGroup.md)||
|startDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|status|String| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|tenantId|String| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|type|String| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|

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

