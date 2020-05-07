---
title: "userExperienceAnalyticsCategory resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsCategory resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List metricValues](../api/userexperienceanalyticscategory-list-metricvalues.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|Get the userExperienceAnalyticsMetrics from the metricValues navigation property.|
|[Create metricValues](../api/userexperienceanalyticscategory-post-metricvalues.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Create a new metricValues object.|
|[Delete metricValues](../api/userexperienceanalyticscategory-delete-metricvalues.md)|None|Delete a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[Update metricValues](../api/userexperienceanalyticscategory-update-metricvalues.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Update the properties of a metricValues object.|
|[Get userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Read the properties and relationships of a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|insights|[userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|metricValues|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "String (identifier)",
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
    }
  ]
}
```

