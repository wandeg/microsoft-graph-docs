---
title: "threatAssessmentResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# threatAssessmentResult resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List threatAssessmentResults](../api/threatassessmentresult-list.md)|[threatAssessmentResult](../resources/threatassessmentresult.md) collection|List properties and relationships of the [threatAssessmentResult](../resources/threatassessmentresult.md) objects.|
|[Get threatAssessmentResult](../api/threatassessmentresult-get.md)|[threatAssessmentResult](../resources/threatassessmentresult.md)|Read properties and relationships of the [threatAssessmentResult](../resources/threatassessmentresult.md) object.|
|[Create threatAssessmentResult](../api/threatassessmentresult-create.md)|[threatAssessmentResult](../resources/threatassessmentresult.md)|Create a new [threatAssessmentResult](../resources/threatassessmentresult.md) object.|
|[Delete threatAssessmentResult](../api/threatassessmentresult-delete.md)|None|Deletes a [threatAssessmentResult](../resources/threatassessmentresult.md).|
|[Update threatAssessmentResult](../api/threatassessmentresult-update.md)|[threatAssessmentResult](../resources/threatassessmentresult.md)|Update the properties of a [threatAssessmentResult](../resources/threatassessmentresult.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|message|String||
|resultType|Enumeration|. Possible values are: `checkPolicy`, `rescan`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.threatAssessmentResult",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.threatAssessmentResult",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "resultType": "String",
  "message": "String"
}
```

