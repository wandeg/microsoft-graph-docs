---
title: "userExperienceAnalyticsInsight resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsInsight resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|insightId|String|The unique identifier of the user experience analytics insight.|
|severity|userExperienceAnalyticsInsightSeverity|The value of the user experience analytics insight. Possible values are: `none`, `informational`, `warning`, `error`.|
|userExperienceAnalyticsMetricId|String|The unique identifier of the user experience analytics insight.|
|values|[userExperienceAnalyticsInsightValue](../resources/userexperienceanalyticsinsightvalue.md) collection|The value of the user experience analytics insight.|

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

