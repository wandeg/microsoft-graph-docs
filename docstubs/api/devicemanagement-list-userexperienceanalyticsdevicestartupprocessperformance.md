---
title: "List userExperienceAnalyticsDeviceStartupProcessPerformance"
description: "Get the userExperienceAnalyticsDeviceStartupProcessPerformances from the userExperienceAnalyticsDeviceStartupProcessPerformance navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userExperienceAnalyticsDeviceStartupProcessPerformance

Namespace: microsoft.graph

Get the userExperienceAnalyticsDeviceStartupProcessPerformances from the userExperienceAnalyticsDeviceStartupProcessPerformance navigation property.

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
GET /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
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
If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userexperienceanalyticsdevicestartupprocessperformance"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.userexperienceanalyticsdevicestartupprocessperformance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 399

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
      "id": "67b98697-8697-67b9-9786-b9679786b967",
      "processName": "Process Name value",
      "productName": "Product Name value",
      "publisher": "Publisher value",
      "deviceCount": 11,
      "medianImpactInMs": 0,
      "totalImpactInMs": 15
    }
  ]
}
```

