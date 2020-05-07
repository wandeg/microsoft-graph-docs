---
title: "userExperienceAnalyticsBaseline resource type"
description: "The user experience analytics baseline entity contains baseline values against which to compare the user experience analytics scores."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsBaseline resource type


Namespace: microsoft.graph

The user experience analytics baseline entity contains baseline values against which to compare the user experience analytics scores.

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
|createdDateTime|DateTimeOffset|The date the custom baseline was created.|
|displayName|String|The name of the user experience analytics baseline.|
|id|String|The unique identifier of the user experience analytics baseline.|
|isBuiltIn|Boolean|Signifies if the current baseline is the commercial median baseline or a custom baseline.|
|overallScore|Int32|The overall score of the user experience analytics baseline.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|bestPracticesMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|The user experience analytics best practices metrics.|
|deviceBootPerformanceMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|The user experience analytics device boot performance metrics.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsBaseline",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsBaseline",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": "Integer",
  "isBuiltIn": "Boolean",
  "createdDateTime": "String (timestamp)"
}
```

