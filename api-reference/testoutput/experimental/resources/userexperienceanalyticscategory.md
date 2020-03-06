---
title: "userExperienceAnalyticsCategory resource type"
description: "The user experience analytics category entity contains the scores and insights for the various metrics of a category."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userExperienceAnalyticsCategory resource type


Namespace: microsoft.graph

The user experience analytics category entity contains the scores and insights for the various metrics of a category.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userExperienceAnalyticsCategory](../api/userexperienceanalyticscategory-get.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.|
|[Update userExperienceAnalyticsCategory](../api/userexperienceanalyticscategory-update.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Update the properties of a [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.|
|[List metricValues](../api/userexperienceanalyticscategory-list-metricvalues.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|Get the userExperienceAnalyticsMetrics from the metricValues navigation property.|
|[Add metricValues](../api/userexperienceanalyticscategory-post-metricvalues.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Add metricValues by posting to the metricValues collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|insights|[userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection|The insights for the user experience analytics category.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|metricValues|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|The metric values for the user experience analytics category.|

## JSON representation
Here is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "String",
      "insightId": "String",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ],
      "severity": "String"
    }
  ]
}
```

