---
title: "Update userExperienceAnalyticsDeviceStartupProcessPerformance"
description: "Update the properties of a userExperienceAnalyticsDeviceStartupProcessPerformance object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userExperienceAnalyticsDeviceStartupProcessPerformance

Namespace: microsoft.graph

Update the properties of a userExperienceAnalyticsDeviceStartupProcessPerformance object.

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
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|processName|String|**TODO: Add Description**|
|productName|String|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|
|deviceCount|Int64|**TODO: Add Description**|
|medianImpactInMs|Int32|**TODO: Add Description**|
|totalImpactInMs|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userexperienceanalyticsdevicestartupprocessperformance"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
Content-Type: application/json
Content-length: 274

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "deviceCount": "Integer",
  "medianImpactInMs": "Integer",
  "totalImpactInMs": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "id": "1cbb67fa-67fa-1cbb-fa67-bb1cfa67bb1c",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "deviceCount": "Integer",
  "medianImpactInMs": "Integer",
  "totalImpactInMs": "Integer"
}
```

