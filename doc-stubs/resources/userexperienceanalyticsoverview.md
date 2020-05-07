---
title: "userExperienceAnalyticsOverview resource type"
description: "The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsOverview resource type


Namespace: microsoft.graph

The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bestPracticesHealthState|userExperienceAnalyticsHealthState|The current health state of the user experience analytics 'BestPractices' category. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|bestPracticesOverallScore|Int32|The user experience analytics best practices overall score.|
|deviceBootPerformanceHealthState|userExperienceAnalyticsHealthState|The current health state of the user experience analytics 'BootPerformance' category. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|deviceBootPerformanceOverallScore|Int32|The user experience analytics device boot performance overall score.|
|id|String|The unique identifier of the user experience analytics overview.|
|insights|[userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection|The user experience analytics insights.|
|overallScore|Int32|The user experience analytics overall score.|
|state|userExperienceAnalyticsHealthState|The current health state of the user experience analytics overview. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsOverview",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsOverview",
  "id": "String (identifier)",
  "overallScore": "Integer",
  "deviceBootPerformanceOverallScore": "Integer",
  "bestPracticesOverallScore": "Integer",
  "insights": [
    {
      "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsInsight"
    }
  ],
  "state": "String",
  "deviceBootPerformanceHealthState": "String",
  "bestPracticesHealthState": "String"
}
```

