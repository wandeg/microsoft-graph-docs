---
title: "userExperienceAnalyticsInsight resource type"
description: "The user experience analytics insight is the recomendation to improve the user experience analytics score."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# userExperienceAnalyticsInsight resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics insight is the recomendation to improve the user experience analytics score.

## Properties

| Property                        | Type                                                                                                  | Description                                                     |
| :------------------------------ | :---------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------- |
| insightId                       | String                                                                                                | The unique identifier of the user experience analytics insight. |
| severity                        | String                                                                                                | The value of the user experience analytics insight.             |
| userExperienceAnalyticsMetricId | String                                                                                                | The unique identifier of the user experience analytics insight. |
| values                          | [userExperienceAnalyticsInsightValue](../resources/userexperienceanalyticsinsightvalue.md) collection | The value of the user experience analytics insight.             |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
  "insightId": "String",
  "severity": "none | informational | warning | error",
  "userExperienceAnalyticsMetricId": "String",
  "values": [{"@odata.type": "microsoft.graph.userExperienceAnalyticsInsightValue"}]
}
```