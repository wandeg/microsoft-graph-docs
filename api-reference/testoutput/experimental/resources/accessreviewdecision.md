---
title: "accessReviewDecision resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# accessReviewDecision resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get accessReviewDecision](../api/accessreviewdecision-get.md)|[accessReviewDecision](../resources/accessReviewDecision.md)|Read properties and relationships of the [accessReviewDecision](../resources/accessreviewdecision.md) object.|
|[Delete accessReviewDecision](../api/accessreviewdecision-delete.md)|None|Deletes a [accessReviewDecision](../resources/accessreviewdecision.md).|
|[Update accessReviewDecision](../api/accessreviewdecision-update.md)|[accessReviewDecision](../resources/accessReviewDecision.md)|Update the properties of a [accessReviewDecision](../resources/accessreviewdecision.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessRecommendation|String||
|accessReviewId|String||
|appliedBy|[userIdentity](../resources/userIdentity.md)||
|appliedDateTime|DateTimeOffset||
|applyResult|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|justification|String||
|reviewedBy|[userIdentity](../resources/userIdentity.md)||
|reviewedDateTime|DateTimeOffset||
|reviewResult|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewDecision",
  "id": "String (identifier)",
  "accessReviewId": "String",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String",
  "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "appliedDateTime": "String (timestamp)",
  "applyResult": "String",
  "accessRecommendation": "String"
}
```

