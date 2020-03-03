---
title: "List restrictedAppsViolations"
description: "List properties and relationships of the restrictedAppsViolation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List restrictedAppsViolations

Namespace: microsoft.graph

List properties and relationships of the [restrictedAppsViolation](../resources/restrictedappsviolation.md) objects.

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
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/restrictedappsviolation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_restrictedappsviolation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.restrictedappsviolation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 693

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.restrictedAppsViolation",
      "id": "ba4be45e-e45e-ba4b-5ee4-4bba5ee44bba",
      "userId": "User Id value",
      "userName": "User Name value",
      "managedDeviceId": "Managed Device Id value",
      "deviceName": "Device Name value",
      "deviceConfigurationId": "Device Configuration Id value",
      "deviceConfigurationName": "Device Configuration Name value",
      "platformType": "String",
      "restrictedAppsState": "String",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.managedDeviceReportedApp",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```

