---
title: "userExperienceAnalyticsBaseline resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsBaseline resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceBootPerformanceMetrics](../api/userexperienceanalyticsbaseline-list-devicebootperformancemetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection|Get the userExperienceAnalyticsCategories from the deviceBootPerformanceMetrics navigation property.|
|[Add deviceBootPerformanceMetrics](../api/userexperienceanalyticsbaseline-post-devicebootperformancemetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Add deviceBootPerformanceMetrics by posting to the deviceBootPerformanceMetrics collection.|
|[Remove deviceBootPerformanceMetrics](../api/userexperienceanalyticsbaseline-delete-devicebootperformancemetrics.md)|None|Remove a [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.|
|[List bestPracticesMetrics](../api/userexperienceanalyticsbaseline-list-bestpracticesmetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection|Get the userExperienceAnalyticsCategories from the bestPracticesMetrics navigation property.|
|[Add bestPracticesMetrics](../api/userexperienceanalyticsbaseline-post-bestpracticesmetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Add bestPracticesMetrics by posting to the bestPracticesMetrics collection.|
|[Remove bestPracticesMetrics](../api/userexperienceanalyticsbaseline-delete-bestpracticesmetrics.md)|None|Remove a [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isBuiltIn|Boolean|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|bestPracticesMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|**TODO: Add Description**|
|deviceBootPerformanceMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBaseline",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "String (identifier)",
  "displayName": "String",
  "isBuiltIn": "Boolean",
  "createdDateTime": "String (timestamp)"
}
```

