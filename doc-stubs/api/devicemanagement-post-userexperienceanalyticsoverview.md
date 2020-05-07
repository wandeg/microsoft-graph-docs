---
title: "Create userExperienceAnalyticsOverview"
description: "Create a new userExperienceAnalyticsOverview object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userExperienceAnalyticsOverview

Namespace: microsoft.graph

Create a new userExperienceAnalyticsOverview object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsOverview
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|The unique identifier of the user experience analytics overview.|
|overallScore|Int32|The user experience analytics overall score.|
|deviceBootPerformanceOverallScore|Int32|The user experience analytics device boot performance overall score.|
|bestPracticesOverallScore|Int32|The user experience analytics best practices overall score.|
|insights|[userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection|The user experience analytics insights.|
|state|userExperienceAnalyticsHealthState|The current health state of the user experience analytics overview. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|deviceBootPerformanceHealthState|userExperienceAnalyticsHealthState|The current health state of the user experience analytics 'BootPerformance' category. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|bestPracticesHealthState|userExperienceAnalyticsHealthState|The current health state of the user experience analytics 'BestPractices' category. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## Response

If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsoverview_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-Type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsOverview",
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

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.userexperienceanalyticsoverview"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsOverview",
  "id": "144343ae-43ae-1443-ae43-4314ae434314",
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

