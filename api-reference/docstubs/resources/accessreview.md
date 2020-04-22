---
title: "accessReview resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# accessReview resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessReviews](../api/accessreview-list.md)|[accessReview](../resources/accessreview.md) collection|Get a list of the [accessReview](../resources/accessreview.md) objects and their properties.|
|[Get accessReview](../api/accessreview-get.md)|[accessReview](../resources/accessreview.md)|Read properties and relationships of an [accessReview](../resources/accessreview.md) object.|
|[Create accessReview](../api/accessreview-post-accessreviews.md)|[accessReview](../resources/accessreview.md)|Create a new [accessReview](../resources/accessreview.md) object.|
|[Delete accessReview](../api/accessreview-delete.md)|None|Deletes an [accessReview](../resources/accessreview.md).|
|[Update accessReview](../api/accessreview-update.md)|[accessReview](../resources/accessreview.md)|Update the properties of a [accessReview](../resources/accessreview.md) object.|
|[stop](../api/accessreview-stop.md)|None|**TODO: Add Description**|
|[sendReminder](../api/accessreview-sendreminder.md)|None|**TODO: Add Description**|
|[resetDecisions](../api/accessreview-resetdecisions.md)|None|**TODO: Add Description**|
|[applyDecisions](../api/accessreview-applydecisions.md)|None|**TODO: Add Description**|
|[List reviewers](../api/accessreview-list-reviewers.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md) collection|Get the accessReviewReviewers from the reviewers navigation property.|
|[Create reviewers](../api/accessreview-post-reviewers.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md)|Create a new reviewers object.|
|[Delete reviewers](../api/accessreview-delete-reviewers.md)|None|Delete a reviewers object.|
|[Update reviewers](../api/accessreview-update-reviewers.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md)|Update the properties of a reviewers object.|
|[Get accessReviewReviewer](../api/accessreviewreviewer-get.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md)|Read properties and relationships of an [accessReviewReviewer](../resources/accessreviewreviewer.md) object.|
|[List decisions](../api/accessreview-list-decisions.md)|[accessReviewDecision](../resources/accessreviewdecision.md) collection|Get the accessReviewDecisions from the decisions navigation property.|
|[Create decisions](../api/accessreview-post-decisions.md)|[accessReviewDecision](../resources/accessreviewdecision.md)|Create a new decisions object.|
|[Delete decisions](../api/accessreview-delete-decisions.md)|None|Delete a decisions object.|
|[Update decisions](../api/accessreview-update-decisions.md)|[accessReviewDecision](../resources/accessreviewdecision.md)|Update the properties of a decisions object.|
|[Get accessReviewDecision](../api/accessreviewdecision-get.md)|[accessReviewDecision](../resources/accessreviewdecision.md)|Read properties and relationships of an [accessReviewDecision](../resources/accessreviewdecision.md) object.|
|[List myDecisions](../api/accessreview-list-mydecisions.md)|[accessReviewDecision](../resources/accessreviewdecision.md) collection|Get the accessReviewDecisions from the myDecisions navigation property.|
|[Create myDecisions](../api/accessreview-post-mydecisions.md)|[accessReviewDecision](../resources/accessreviewdecision.md)|Create a new myDecisions object.|
|[Delete myDecisions](../api/accessreview-delete-mydecisions.md)|None|Delete a myDecisions object.|
|[Update myDecisions](../api/accessreview-update-mydecisions.md)|[accessReviewDecision](../resources/accessreviewdecision.md)|Update the properties of a myDecisions object.|
|[Get accessReviewDecision](../api/accessreviewdecision-get.md)|[accessReviewDecision](../resources/accessreviewdecision.md)|Read properties and relationships of an [accessReviewDecision](../resources/accessreviewdecision.md) object.|
|[List instances](../api/accessreview-list-instances.md)|[accessReview](../resources/accessreview.md) collection|Get the accessReviews from the instances navigation property.|
|[Create instances](../api/accessreview-post-instances.md)|[accessReview](../resources/accessreview.md)|Create a new instances object.|
|[Delete instances](../api/accessreview-delete-instances.md)|None|Delete an instances object.|
|[Update instances](../api/accessreview-update-instances.md)|[accessReview](../resources/accessreview.md)|Update the properties of an instances object.|
|[Get accessReview](../api/accessreview-get.md)|[accessReview](../resources/accessreview.md)|Read properties and relationships of an [accessReview](../resources/accessreview.md) object.|

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
Here is a JSON representation of the resource.
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

