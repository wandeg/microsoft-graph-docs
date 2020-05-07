---
title: "Create userExperienceAnalyticsDeviceStartupHistory"
description: "Create a new userExperienceAnalyticsDeviceStartupHistory object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userExperienceAnalyticsDeviceStartupHistory

Namespace: microsoft.graph

Create a new userExperienceAnalyticsDeviceStartupHistory object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|The unique identifier of the user experience analytics device startup history.|
|deviceId|String|The user experience analytics device id.|
|startTime|DateTimeOffset|The user experience analytics device boot start time.|
|coreBootTimeInMs|Int32|The user experience analytics device core boot time in milliseconds.|
|groupPolicyBootTimeInMs|Int32|The User experience analytics Device group policy boot time in milliseconds.|
|featureUpdateBootTimeInMs|Int32|The user experience analytics device feature update time in milliseconds.|
|totalBootTimeInMs|Int32|The user experience analytics device total boot time in milliseconds.|
|groupPolicyLoginTimeInMs|Int32|The User experience analytics Device group policy login time in milliseconds.|
|coreLoginTimeInMs|Int32|The user experience analytics device core login time in milliseconds.|
|responsiveDesktopTimeInMs|Int32|The user experience analytics responsive desktop time in milliseconds.|
|totalLoginTimeInMs|Int32|The user experience analytics device total login time in milliseconds.|
|isFirstLogin|Boolean|The user experience analytics device first login.|
|isFeatureUpdate|Boolean|The user experience analytics device boot record is a feature update.|
|operatingSystemVersion|String|The user experience analytics device boot record's operating system version.|



## Response

If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsdevicestartuphistory_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-Type: application/json
Content-length: 577

{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsDeviceStartupHistory",
  "deviceId": "String",
  "startTime": "String (timestamp)",
  "coreBootTimeInMs": "Integer",
  "groupPolicyBootTimeInMs": "Integer",
  "featureUpdateBootTimeInMs": "Integer",
  "totalBootTimeInMs": "Integer",
  "groupPolicyLoginTimeInMs": "Integer",
  "coreLoginTimeInMs": "Integer",
  "responsiveDesktopTimeInMs": "Integer",
  "totalLoginTimeInMs": "Integer",
  "isFirstLogin": "Boolean",
  "isFeatureUpdate": "Boolean",
  "operatingSystemVersion": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.userexperienceanalyticsdevicestartuphistory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsDeviceStartupHistory",
  "id": "62ace4c2-e4c2-62ac-c2e4-ac62c2e4ac62",
  "deviceId": "String",
  "startTime": "String (timestamp)",
  "coreBootTimeInMs": "Integer",
  "groupPolicyBootTimeInMs": "Integer",
  "featureUpdateBootTimeInMs": "Integer",
  "totalBootTimeInMs": "Integer",
  "groupPolicyLoginTimeInMs": "Integer",
  "coreLoginTimeInMs": "Integer",
  "responsiveDesktopTimeInMs": "Integer",
  "totalLoginTimeInMs": "Integer",
  "isFirstLogin": "Boolean",
  "isFeatureUpdate": "Boolean",
  "operatingSystemVersion": "String"
}
```

