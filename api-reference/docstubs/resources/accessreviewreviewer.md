---
title: "accessReviewReviewer resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# accessReviewReviewer resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get accessReviewReviewer](../api/accessreviewreviewer-get.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md)|Read properties and relationships of an [accessReviewReviewer](../resources/accessreviewreviewer.md) object.|
|[Update accessReviewReviewer](../api/accessreviewreviewer-update.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md)|Update the properties of a [accessReviewReviewer](../resources/accessreviewreviewer.md) object.|
|[List reviewers](../api/accessreview-list-reviewers.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md) collection|Get the accessReviewReviewers from the reviewers navigation property.|
|[Create reviewers](../api/accessreview-post-reviewers.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md)|Create a new reviewers object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewReviewer",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewer",
  "id": "String (identifier)",
  "displayName": "String",
  "userPrincipalName": "String"
}
```

