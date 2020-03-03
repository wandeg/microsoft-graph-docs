---
title: "classificationJobResponse resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# classificationJobResponse resource type




Inherits from [jobResponseBase](../resources/jobResponseBase.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List classificationJobResponses](../api/classificationjobresponse-list.md)|[classificationJobResponse](../resources/classificationJobResponse.md) collection|List properties and relationships of the [classificationJobResponse](../resources/classificationjobresponse.md) objects.|
|[Get classificationJobResponse](../api/classificationjobresponse-get.md)|[classificationJobResponse](../resources/classificationJobResponse.md)|Read properties and relationships of the [classificationJobResponse](../resources/classificationjobresponse.md) object.|
|[Create classificationJobResponse](../api/classificationjobresponse-create.md)|[classificationJobResponse](../resources/classificationJobResponse.md)|Create a new [classificationJobResponse](../resources/classificationjobresponse.md) object.|
|[Delete classificationJobResponse](../api/classificationjobresponse-delete.md)|None|Deletes a [classificationJobResponse](../resources/classificationjobresponse.md).|
|[Update classificationJobResponse](../api/classificationjobresponse-update.md)|[classificationJobResponse](../resources/classificationJobResponse.md)|Update the properties of a [classificationJobResponse](../resources/classificationjobresponse.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|endDateTime|DateTimeOffset| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|error|[classificationError](../resources/classificationError.md)| Inherited from [jobResponseBase](../resources/jobResponseBase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|result|[detectedSensitiveContentWrapper](../resources/detectedSensitiveContentWrapper.md)||
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
  "@odata.type": "microsoft.graph.classificationJobResponse",
  "baseType": "microsoft.graph.jobResponseBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.classificationJobResponse",
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
    "@odata.type": "microsoft.graph.detectedSensitiveContentWrapper"
  }
}
```

