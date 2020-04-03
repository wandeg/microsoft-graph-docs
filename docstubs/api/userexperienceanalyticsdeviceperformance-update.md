---
title: "Update userExperienceAnalyticsDevicePerformance"
description: "Update the properties of a userExperienceAnalyticsDevicePerformance object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userExperienceAnalyticsDevicePerformance

Namespace: microsoft.graph

Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) object.

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
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deviceName|String||
|model|String||
|manufacturer|String||
|diskType|Enumeration| Possible values are: `unkown`, `hdd`, `ssd`.|
|operatingSystemVersion|String||
|bootScore|Int32||
|coreBootTimeInMs|Int32||
|groupPolicyBootTimeInMs|Int32||
|healthStatus|Enumeration| Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|loginScore|Int32||
|coreLoginTimeInMs|Int32||
|groupPolicyLoginTimeInMs|Int32||
|deviceCount|Int64||
|responsiveDesktopTimeInMs|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_userexperienceanalyticsdeviceperformance"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
Content-type: application/json
Content-length: 522

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
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
Content-Length: 571

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "id": "e7bfb4e7-b4e7-e7bf-e7b4-bfe7e7b4bfe7",
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
```

