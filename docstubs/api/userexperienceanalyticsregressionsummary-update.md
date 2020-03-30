---
title: "Update userExperienceAnalyticsRegressionSummary"
description: "Update the properties of a userExperienceAnalyticsRegressionSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userExperienceAnalyticsRegressionSummary

Namespace: microsoft.graph

Update the properties of a [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object.

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
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsRegressionSummary](../resources/userexperienceanalyticsregressionsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_userexperienceanalyticsregressionsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary
Content-type: application/json
Content-length: 82

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary"
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
Content-Length: 131

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "c651c142-c142-c651-42c1-51c642c151c6"
}
```

