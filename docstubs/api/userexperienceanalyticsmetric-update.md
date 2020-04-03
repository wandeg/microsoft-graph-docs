---
title: "Update userExperienceAnalyticsMetric"
description: "Update the properties of a userExperienceAnalyticsMetric object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userExperienceAnalyticsMetric

Namespace: microsoft.graph

Update the properties of a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.

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
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|Double||
|unit|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_userexperienceanalyticsmetric"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
Content-type: application/json
Content-length: 118

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": "Double",
  "unit": "Unit value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 167

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "6d432754-2754-6d43-5427-436d5427436d",
  "value": "Double",
  "unit": "Unit value"
}
```

