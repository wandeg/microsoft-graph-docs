---
title: "userExperienceAnalyticsInsight resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userExperienceAnalyticsInsight resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|insightId|String||
|severity|Enumeration| Possible values are: `none`, `informational`, `warning`, `error`.|
|userExperienceAnalyticsMetricId|String||
|values|[userExperienceAnalyticsInsightValue](../resources/userexperienceanalyticsinsightvalue.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
  "userExperienceAnalyticsMetricId": "String",
  "insightId": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble",
      "value": "Double"
    }
  ],
  "severity": "String"
}
```

