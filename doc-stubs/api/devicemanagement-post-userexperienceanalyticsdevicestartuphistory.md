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
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deviceId|String|**TODO: Add Description**|
|startTime|DateTimeOffset|**TODO: Add Description**|
|coreBootTimeInMs|Int32|**TODO: Add Description**|
|groupPolicyBootTimeInMs|Int32|**TODO: Add Description**|
|featureUpdateBootTimeInMs|Int32|**TODO: Add Description**|
|totalBootTimeInMs|Int32|**TODO: Add Description**|
|groupPolicyLoginTimeInMs|Int32|**TODO: Add Description**|
|coreLoginTimeInMs|Int32|**TODO: Add Description**|
|responsiveDesktopTimeInMs|Int32|**TODO: Add Description**|
|totalLoginTimeInMs|Int32|**TODO: Add Description**|
|isFirstLogin|Boolean|**TODO: Add Description**|
|isFeatureUpdate|Boolean|**TODO: Add Description**|
|operatingSystemVersion|String|**TODO: Add Description**|



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
Content-length: 559

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
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
  "@odata.type": "microsoft.graph.userexperienceanalyticsdevicestartuphistory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "8fccbc3f-bc3f-8fcc-3fbc-cc8f3fbccc8f",
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

