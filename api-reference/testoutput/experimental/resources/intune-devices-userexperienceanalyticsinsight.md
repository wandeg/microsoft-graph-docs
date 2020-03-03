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
|insightId|String|The unique identifier of the user experience analytics insight.|
|severity|Enumeration|The value of the user experience analytics insight. Possible values are: `none`, `informational`, `warning`, `error`.|
|userExperienceAnalyticsMetricId|String|The unique identifier of the user experience analytics insight.|
|values|[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection|The value of the user experience analytics insight.|

## Relationships
None

## JSON Representation
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

