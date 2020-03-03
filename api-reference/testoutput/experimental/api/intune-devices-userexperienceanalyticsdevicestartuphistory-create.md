---
title: "Create userExperienceAnalyticsDeviceStartupHistory"
description: "Create a new userExperienceAnalyticsDeviceStartupHistory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create userExperienceAnalyticsDeviceStartupHistory

Namespace: microsoft.graph

Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.

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
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deviceId|String|The user experience analytics device id.|
|startTime|DateTimeOffset|The user experience analytics device boot start time.|
|coreBootTimeInMs|Int32|The user experience analytics device core boot time in milliseconds.|
|groupPolicyBootTimeInMs|Int32|The User experience analytics Device group policy boot time in milliseconds.|
|featureUpdateBootTimeInMs|Int32|The user experience analytics device feature update time in milliseconds.|
|totalBootTimeInMs|Int32|The user experience analytics device total boot time in milliseconds.|
|groupPolicyLoginTimeInMs|Int32|The User experience analytics Device group policy login time in milliseconds.|
|coreLoginTimeInMs|Int32|The user experience analytics device core login time in milliseconds.|
|totalLoginTimeInMs|Int32|The user experience analytics device total login time in milliseconds.|
|isFirstLogin|Boolean|The user experience analytics device first login.|
|isFeatureUpdate|Boolean|The user experience analytics device boot record is a feature update.|
|operatingSystemVersion|String|The user experience analytics device boot record's operating system version.|



## Response
If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsdevicestartuphistory_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 498

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:02:49.6370207+03:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userexperienceanalyticsdevicestartuphistory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 547

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "3431c76a-c76a-3431-6ac7-31346ac73134",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:02:49.6370207+03:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value"
}
```

