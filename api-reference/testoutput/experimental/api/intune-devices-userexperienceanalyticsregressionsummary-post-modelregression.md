---
title: "Add modelRegression"
description: "Add modelRegression by posting to the modelRegression collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add modelRegression

Namespace: microsoft.graph

Add modelRegression by posting to the modelRegression collection.

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
POST /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|Double|The value of the user experience analytics metric.|
|unit|String|The unit of the user experience analytics metric.|



## Response
If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsmetric_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
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
  "id": "b8a03256-3256-b8a0-5632-a0b85632a0b8",
  "value": "Double",
  "unit": "Unit value"
}
```

