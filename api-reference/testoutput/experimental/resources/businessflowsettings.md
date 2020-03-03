---
title: "businessFlowSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# businessFlowSettings resource type




Inherits from [accessReviewSettings](../resources/accessReviewSettings.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessRecommendationsEnabled|Boolean| Inherited from [accessReviewSettings](../resources/accessReviewSettings.md)|
|activityDurationInDays|Int32| Inherited from [accessReviewSettings](../resources/accessReviewSettings.md)|
|autoApplyReviewResultsEnabled|Boolean| Inherited from [accessReviewSettings](../resources/accessReviewSettings.md)|
|autoReviewEnabled|Boolean| Inherited from [accessReviewSettings](../resources/accessReviewSettings.md)|
|autoReviewSettings|[autoReviewSettings](../resources/autoReviewSettings.md)| Inherited from [accessReviewSettings](../resources/accessReviewSettings.md)|
|durationInDays|Int32||
|justificationRequiredOnApproval|Boolean| Inherited from [accessReviewSettings](../resources/accessReviewSettings.md)|
|mailNotificationsEnabled|Boolean| Inherited from [accessReviewSettings](../resources/accessReviewSettings.md)|
|recurrenceSettings|[accessReviewRecurrenceSettings](../resources/accessReviewRecurrenceSettings.md)| Inherited from [accessReviewSettings](../resources/accessReviewSettings.md)|
|remindersEnabled|Boolean| Inherited from [accessReviewSettings](../resources/accessReviewSettings.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.businessFlowSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.businessFlowSettings",
  "mailNotificationsEnabled": true,
  "remindersEnabled": true,
  "justificationRequiredOnApproval": true,
  "recurrenceSettings": {
    "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings",
    "recurrenceType": "String",
    "recurrenceEndType": "String",
    "durationInDays": 1024,
    "recurrenceCount": 1024
  },
  "autoReviewEnabled": true,
  "activityDurationInDays": 1024,
  "autoReviewSettings": {
    "@odata.type": "microsoft.graph.autoReviewSettings",
    "notReviewedResult": "String"
  },
  "autoApplyReviewResultsEnabled": true,
  "accessRecommendationsEnabled": true,
  "durationInDays": 1024
}
```

