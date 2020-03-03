---
title: "accessReviewSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# accessReviewSettings resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessRecommendationsEnabled|Boolean||
|activityDurationInDays|Int32||
|autoApplyReviewResultsEnabled|Boolean||
|autoReviewEnabled|Boolean||
|autoReviewSettings|[autoReviewSettings](../resources/autoReviewSettings.md)||
|justificationRequiredOnApproval|Boolean||
|mailNotificationsEnabled|Boolean||
|recurrenceSettings|[accessReviewRecurrenceSettings](../resources/accessReviewRecurrenceSettings.md)||
|remindersEnabled|Boolean||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewSettings",
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
  "accessRecommendationsEnabled": true
}
```

