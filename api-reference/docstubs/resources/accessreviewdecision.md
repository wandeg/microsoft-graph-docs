---
title: "accessReviewDecision resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# accessReviewDecision resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessReviewDecisions](../api/accessreviewdecision-list.md)|[accessReviewDecision](../resources/accessreviewdecision.md) collection|Get a list of the [accessReviewDecision](../resources/accessreviewdecision.md) objects and their properties.|
|[Get accessReviewDecision](../api/accessreviewdecision-get.md)|[accessReviewDecision](../resources/accessreviewdecision.md)|Read properties and relationships of an [accessReviewDecision](../resources/accessreviewdecision.md) object.|
|[Create accessReviewDecision](../api/accessreviewdecision-post-accessreviewdecisions.md)|[accessReviewDecision](../resources/accessreviewdecision.md)|Create a new [accessReviewDecision](../resources/accessreviewdecision.md) object.|
|[Delete accessReviewDecision](../api/accessreviewdecision-delete.md)|None|Deletes an [accessReviewDecision](../resources/accessreviewdecision.md).|
|[Update accessReviewDecision](../api/accessreviewdecision-update.md)|[accessReviewDecision](../resources/accessreviewdecision.md)|Update the properties of a [accessReviewDecision](../resources/accessreviewdecision.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessRecommendation|String|**TODO: Add Description**|
|accessReviewId|String|**TODO: Add Description**|
|appliedBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|appliedDateTime|DateTimeOffset|**TODO: Add Description**|
|applyResult|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|justification|String|**TODO: Add Description**|
|reviewedBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|reviewedDateTime|DateTimeOffset|**TODO: Add Description**|
|reviewResult|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "baseType": "",
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

