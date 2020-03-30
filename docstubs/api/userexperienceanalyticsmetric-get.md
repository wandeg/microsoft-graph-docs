---
title: "Get userExperienceAnalyticsMetric"
description: "Read properties and relationships of the userExperienceAnalyticsMetric object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get userExperienceAnalyticsMetric

Namespace: microsoft.graph

Read properties and relationships of the [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression/{userExperienceAnalyticsMetricId}
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression/{userExperienceAnalyticsMetricId}
GET /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userexperienceanalyticsmetric"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetric"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
    "id": "d523b42c-b42c-d523-2cb4-23d52cb423d5",
    "value": "Double",
    "unit": "Unit value"
  }
}
```

