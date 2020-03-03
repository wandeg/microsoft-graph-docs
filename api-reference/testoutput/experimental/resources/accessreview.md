---
title: "accessReview resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# accessReview resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessReviews](../api/accessreview-list.md)|[accessReview](../resources/accessReview.md) collection|List properties and relationships of the [accessReview](../resources/accessreview.md) objects.|
|[Get accessReview](../api/accessreview-get.md)|[accessReview](../resources/accessReview.md)|Read properties and relationships of the [accessReview](../resources/accessreview.md) object.|
|[Create accessReview](../api/accessreview-post-accessreviews.md)|[accessReview](../resources/accessReview.md)|Create a new [accessReview](../resources/accessreview.md) object.|
|[Delete accessReview](../api/accessreview-delete.md)|None|Deletes a [accessReview](../resources/accessreview.md).|
|[Update accessReview](../api/accessreview-update.md)|[accessReview](../resources/accessReview.md)|Update the properties of a [accessReview](../resources/accessreview.md) object.|
|[stop](../api/accessreview-stop.md)|None||
|[sendReminder](../api/accessreview-sendreminder.md)|None||
|[resetDecisions](../api/accessreview-resetdecisions.md)|None||
|[applyDecisions](../api/accessreview-applydecisions.md)|None||
|[List reviewers](../api/accessreview-list-reviewers.md)|[accessReviewReviewer](../resources/accessReviewReviewer.md) collection|Get the accessReviewReviewers from the reviewers navigation property.|
|[Add reviewers](../api/accessreview-post-reviewers.md)|[accessReviewReviewer](../resources/accessReviewReviewer.md)|Add reviewers by posting to the reviewers collection.|
|[List decisions](../api/accessreview-list-decisions.md)|[accessReviewDecision](../resources/accessReviewDecision.md) collection|Get the accessReviewDecisions from the decisions navigation property.|
|[Add decisions](../api/accessreview-post-decisions.md)|[accessReviewDecision](../resources/accessReviewDecision.md)|Add decisions by posting to the decisions collection.|
|[List myDecisions](../api/accessreview-list-mydecisions.md)|[accessReviewDecision](../resources/accessReviewDecision.md) collection|Get the accessReviewDecisions from the myDecisions navigation property.|
|[Add myDecisions](../api/accessreview-post-mydecisions.md)|[accessReviewDecision](../resources/accessReviewDecision.md)|Add myDecisions by posting to the myDecisions collection.|
|[List instances](../api/accessreview-list-instances.md)|[accessReview](../resources/accessReview.md) collection|Get the accessReviews from the instances navigation property.|
|[Add instances](../api/accessreview-post-instances.md)|[accessReview](../resources/accessReview.md)|Add instances by posting to the instances collection.|
|[List instances](../api/accessreview-list-instances.md)|[accessReview](../resources/accessReview.md) collection|Get the accessReviews from the instances navigation property.|
|[Add instances](../api/accessreview-post-instances.md)|[accessReview](../resources/accessReview.md)|Add instances by posting to the instances collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|businessFlowTemplateId|String||
|createdBy|[userIdentity](../resources/userIdentity.md)||
|description|String||
|displayName|String||
|endDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|reviewedEntity|[identity](../resources/identity.md)||
|reviewerType|String||
|settings|[accessReviewSettings](../resources/accessReviewSettings.md)||
|startDateTime|DateTimeOffset||
|status|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|decisions|[accessReviewDecision](../resources/accessReviewDecision.md) collection||
|instances|[accessReview](../resources/accessReview.md) collection||
|myDecisions|[accessReviewDecision](../resources/accessReviewDecision.md) collection||
|reviewers|[accessReviewReviewer](../resources/accessReviewReviewer.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReview",
  "baseType": "microsoft.graph.entity",
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

