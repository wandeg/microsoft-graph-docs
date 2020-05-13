---
title: "accessReview resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessReview resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessReviews](../api/accessreview-list.md)|[accessReview](../resources/accessreview.md) collection|Get a list of the [accessReview](../resources/accessreview.md) objects and their properties.|
|[Get accessReview](../api/accessreview-get.md)|[accessReview](../resources/accessreview.md)|Read the properties and relationships of an [accessReview](../resources/accessreview.md) object.|
|[Create accessReview](../api/accessreview-post-accessreviews.md)|[accessReview](../resources/accessreview.md)|Create a new [accessReview](../resources/accessreview.md) object.|
|[Delete accessReview](../api/accessreview-delete.md)|None|Deletes an [accessReview](../resources/accessreview.md) object.|
|[Update accessReview](../api/accessreview-update.md)|[accessReview](../resources/accessreview.md)|Update the properties of an [accessReview](../resources/accessreview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|businessFlowTemplateId|String|**TODO: Add Description**|
|createdBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|reviewedEntity|[identity](../resources/identity.md)|**TODO: Add Description**|
|reviewerType|String|**TODO: Add Description**|
|settings|[accessReviewSettings](../resources/accessreviewsettings.md)|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|status|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|decisions|[accessReviewDecision](../resources/accessreviewdecision.md) collection|**TODO: Add Description**|
|instances|[accessReview](../resources/accessreview.md) collection|**TODO: Add Description**|
|myDecisions|[accessReviewDecision](../resources/accessreviewdecision.md) collection|**TODO: Add Description**|
|reviewers|[accessReviewReviewer](../resources/accessreviewreviewer.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReview",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReview",
  "id": "String (identifier)",
  "displayName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "status": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "businessFlowTemplateId": "String",
  "reviewerType": "String",
  "description": "String",
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewSettings"
  },
  "reviewedEntity": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

