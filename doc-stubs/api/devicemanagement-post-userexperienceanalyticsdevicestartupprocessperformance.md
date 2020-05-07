---
title: "Create userExperienceAnalyticsDeviceStartupProcessPerformance"
description: "Create a new userExperienceAnalyticsDeviceStartupProcessPerformance object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userExperienceAnalyticsDeviceStartupProcessPerformance

Namespace: microsoft.graph

Create a new userExperienceAnalyticsDeviceStartupProcessPerformance object.

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
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
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

If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsdevicestartupprocessperformance_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
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
  "truncated": true,
  "@odata.type": "microsoft.graph.userexperienceanalyticsdevicestartupprocessperformance"
}
-->
``` http
HTTP/1.1 201 Created
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

