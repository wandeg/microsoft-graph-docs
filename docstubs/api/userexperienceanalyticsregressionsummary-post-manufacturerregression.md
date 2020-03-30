---
title: "Add manufacturerRegression"
description: "Add manufacturerRegression by posting to the manufacturerRegression collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add manufacturerRegression

Namespace: microsoft.graph

Add manufacturerRegression by posting to the manufacturerRegression collection.

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
POST /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|Double||
|unit|String||



## Response
If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsmetric_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression
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
  "truncated": true,
  "@odata.type": "microsoft.graph.userexperienceanalyticsmetric"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 167

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "d523b42c-b42c-d523-2cb4-23d52cb423d5",
  "value": "Double",
  "unit": "Unit value"
}
```

