---
title: "Get userExperienceAnalyticsDeviceStartupHistory"
description: "Read properties and relationships of the userExperienceAnalyticsDeviceStartupHistory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get userExperienceAnalyticsDeviceStartupHistory

Namespace: microsoft.graph

Read properties and relationships of the [userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) object.

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
GET /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
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
If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userexperienceanalyticsdevicestartuphistory"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupHistory"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 631

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
    "id": "c50a8278-8278-c50a-7882-0ac578820ac5",
    "deviceId": "Device Id value",
    "startTime": "2017-01-01T00:01:56.9262257+00:00",
    "coreBootTimeInMs": 0,
    "groupPolicyBootTimeInMs": 7,
    "featureUpdateBootTimeInMs": 9,
    "totalBootTimeInMs": 1,
    "groupPolicyLoginTimeInMs": 8,
    "coreLoginTimeInMs": 1,
    "responsiveDesktopTimeInMs": 9,
    "totalLoginTimeInMs": 2,
    "isFirstLogin": true,
    "isFeatureUpdate": true,
    "operatingSystemVersion": "Operating System Version value"
  }
}
```

