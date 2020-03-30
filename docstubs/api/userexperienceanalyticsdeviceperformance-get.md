---
title: "Get userExperienceAnalyticsDevicePerformance"
description: "Read properties and relationships of the userExperienceAnalyticsDevicePerformance object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get userExperienceAnalyticsDevicePerformance

Namespace: microsoft.graph

Read properties and relationships of the [userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) object.

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
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
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
If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_userexperienceanalyticsdeviceperformance"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDevicePerformance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
    "id": "cf79e859-e859-cf79-59e8-79cf59e879cf",
    "deviceName": "Device Name value",
    "model": "Model value",
    "manufacturer": "Manufacturer value",
    "diskType": "String",
    "operatingSystemVersion": "Operating System Version value",
    "bootScore": 9,
    "coreBootTimeInMs": 0,
    "groupPolicyBootTimeInMs": 7,
    "healthStatus": "String",
    "loginScore": 10,
    "coreLoginTimeInMs": 1,
    "groupPolicyLoginTimeInMs": 8,
    "deviceCount": 11,
    "responsiveDesktopTimeInMs": 9
  }
}
```

