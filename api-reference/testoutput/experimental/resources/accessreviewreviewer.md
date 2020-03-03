---
title: "accessReviewReviewer resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# accessReviewReviewer resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List accessReviewReviewers](../api/accessreviewreviewer-list.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md) collection|List properties and relationships of the [accessReviewReviewer](../resources/accessreviewreviewer.md) objects.|
|[Get accessReviewReviewer](../api/accessreviewreviewer-get.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md)|Read properties and relationships of the [accessReviewReviewer](../resources/accessreviewreviewer.md) object.|
|[Create accessReviewReviewer](../api/accessreviewreviewer-create.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md)|Create a new [accessReviewReviewer](../resources/accessreviewreviewer.md) object.|
|[Delete accessReviewReviewer](../api/accessreviewreviewer-delete.md)|None|Deletes a [accessReviewReviewer](../resources/accessreviewreviewer.md).|
|[Update accessReviewReviewer](../api/accessreviewreviewer-update.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md)|Update the properties of a [accessReviewReviewer](../resources/accessreviewreviewer.md) object.|
|[List reviewers](../api/accessreview-list-reviewers.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md) collection|Get the accessReviewReviewers from the reviewers navigation property.|
|[Add reviewers](../api/accessreview-post-reviewers.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md)|Add reviewers by posting to the reviewers collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewReviewer",
  "baseType": "microsoft.graph.entity",
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

