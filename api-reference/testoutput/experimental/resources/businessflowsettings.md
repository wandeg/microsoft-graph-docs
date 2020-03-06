---
title: "businessFlowSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# businessFlowSettings resource type


Namespace: microsoft.graph




Inherits from [accessReviewSettings](../resources/accessreviewsettings.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessRecommendationsEnabled|Boolean| Inherited from [accessReviewSettings](../resources/accessreviewsettings.md)|
|activityDurationInDays|Int32| Inherited from [accessReviewSettings](../resources/accessreviewsettings.md)|
|autoApplyReviewResultsEnabled|Boolean| Inherited from [accessReviewSettings](../resources/accessreviewsettings.md)|
|autoReviewEnabled|Boolean| Inherited from [accessReviewSettings](../resources/accessreviewsettings.md)|
|autoReviewSettings|[autoReviewSettings](../resources/autoreviewsettings.md)| Inherited from [accessReviewSettings](../resources/accessreviewsettings.md)|
|durationInDays|Int32||
|justificationRequiredOnApproval|Boolean| Inherited from [accessReviewSettings](../resources/accessreviewsettings.md)|
|mailNotificationsEnabled|Boolean| Inherited from [accessReviewSettings](../resources/accessreviewsettings.md)|
|recurrenceSettings|[accessReviewRecurrenceSettings](../resources/accessreviewrecurrencesettings.md)| Inherited from [accessReviewSettings](../resources/accessreviewsettings.md)|
|remindersEnabled|Boolean| Inherited from [accessReviewSettings](../resources/accessreviewsettings.md)|

## Relationships
None

## JSON representation
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

