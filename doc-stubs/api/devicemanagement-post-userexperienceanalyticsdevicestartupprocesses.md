---
title: "Create userExperienceAnalyticsDeviceStartupProcesses"
description: "Create a new userExperienceAnalyticsDeviceStartupProcesses object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userExperienceAnalyticsDeviceStartupProcesses

Namespace: microsoft.graph

Create a new userExperienceAnalyticsDeviceStartupProcesses object.

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
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|managedDeviceId|String|**TODO: Add Description**|
|processName|String|**TODO: Add Description**|
|productName|String|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|
|startupImpactInMs|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcess](../resources/userexperienceanalyticsdevicestartupprocess.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsdevicestartupprocess_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
Content-Type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "managedDeviceId": "String",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "startupImpactInMs": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userexperienceanalyticsdevicestartupprocess"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "id": "58bd4832-4832-58bd-3248-bd583248bd58",
  "managedDeviceId": "String",
  "processName": "String",
  "productName": "String",
  "publisher": "String",
  "startupImpactInMs": "Integer"
}
```

