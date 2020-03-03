---
title: "userExperienceAnalyticsCategory resource type"
description: "The user experience analytics category entity contains the scores and insights for the various metrics of a category."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# userExperienceAnalyticsCategory resource type

The user experience analytics category entity contains the scores and insights for the various metrics of a category.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userExperienceAnalyticsCategory](../api/intune-devices-userexperienceanalyticscategory-get.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userExperienceAnalyticsCategory.md)|Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.|
|[Delete userExperienceAnalyticsCategory](../api/intune-devices-userexperienceanalyticscategory-delete.md)|None|Deletes a [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md).|
|[Update userExperienceAnalyticsCategory](../api/intune-devices-userexperienceanalyticscategory-update.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userExperienceAnalyticsCategory.md)|Update the properties of a [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.|
|[List metricValues](../api/intune-devices-userexperienceanalyticscategory-list-metricvalues.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md) collection|Get the userExperienceAnalyticsMetrics from the metricValues navigation property.|
|[Add metricValues](../api/intune-devices-userexperienceanalyticscategory-post-metricvalues.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md)|Add metricValues by posting to the metricValues collection.|
|[List userExperienceAnalyticsCategories](../api/intune-devices-devicemanagement-list-userexperienceanalyticscategories.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userExperienceAnalyticsCategory.md) collection|Get the userExperienceAnalyticsCategories from the userExperienceAnalyticsCategories navigation property.|
|[Add userExperienceAnalyticsCategories](../api/intune-devices-devicemanagement-post-userexperienceanalyticscategories.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userExperienceAnalyticsCategory.md)|Add userExperienceAnalyticsCategories by posting to the userExperienceAnalyticsCategories collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|insights|[userExperienceAnalyticsInsight](../resources/intune-devices-userExperienceAnalyticsInsight.md) collection|The insights for the user experience analytics category.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|metricValues|[userExperienceAnalyticsMetric](../resources/intune-devices-userExperienceAnalyticsMetric.md) collection|The metric values for the user experience analytics category.|

## JSON Representation
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

