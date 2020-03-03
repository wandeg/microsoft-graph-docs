---
title: "List operatingSystemRegression"
description: "Get the userExperienceAnalyticsMetrics from the operatingSystemRegression navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List operatingSystemRegression

Namespace: microsoft.graph

Get the userExperienceAnalyticsMetrics from the operatingSystemRegression navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userexperienceanalyticsmetric"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.userexperienceanalyticsmetric)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
      "id": "b8a03256-3256-b8a0-5632-a0b85632a0b8",
      "value": "Double",
      "unit": "Unit value"
    }
  ]
}
```

