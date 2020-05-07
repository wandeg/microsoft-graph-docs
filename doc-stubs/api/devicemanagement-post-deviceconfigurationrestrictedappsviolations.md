---
title: "Create deviceConfigurationRestrictedAppsViolations"
description: "Create a new deviceConfigurationRestrictedAppsViolations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceConfigurationRestrictedAppsViolations

Namespace: microsoft.graph

Create a new deviceConfigurationRestrictedAppsViolations object.

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
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [restrictedAppsViolation](../resources/restrictedappsviolation.md) object.

The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/restrictedappsviolation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userId|String|**TODO: Add Description**|
|userName|String|**TODO: Add Description**|
|managedDeviceId|String|**TODO: Add Description**|
|deviceName|String|**TODO: Add Description**|
|deviceConfigurationId|String|**TODO: Add Description**|
|deviceConfigurationName|String|**TODO: Add Description**|
|platformType|policyPlatformType|**TODO: Add Description**. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|restrictedAppsState|restrictedAppsState|**TODO: Add Description**. Possible values are: `prohibitedApps`, `notApprovedApps`.|
|restrictedApps|[managedDeviceReportedApp](../resources/manageddevicereportedapp.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/restrictedappsviolation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_restrictedappsviolation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
Content-Type: application/json
Content-length: 423

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp"
    }
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.restrictedappsviolation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "3060e475-e475-3060-75e4-603075e46030",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp"
    }
  ]
}
```

