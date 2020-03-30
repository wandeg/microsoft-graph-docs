---
title: "List deviceConfigurationRestrictedAppsViolations"
description: "Get the restrictedAppsViolations from the deviceConfigurationRestrictedAppsViolations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceConfigurationRestrictedAppsViolations

Namespace: microsoft.graph

Get the restrictedAppsViolations from the deviceConfigurationRestrictedAppsViolations navigation property.

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
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
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
If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/restrictedappsviolation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_restrictedappsviolation"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
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
      "id": "fca4ecc7-ecc7-fca4-c7ec-a4fcc7eca4fc",
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

