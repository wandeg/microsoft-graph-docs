---
title: "List managedAppRegistrations"
description: "Get the managedAppRegistrations from the managedAppRegistrations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List managedAppRegistrations

Namespace: microsoft.graph

Get the managedAppRegistrations from the managedAppRegistrations navigation property.

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
GET /deviceAppManagement/managedAppRegistrations
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
If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/managedappregistration.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_managedappregistration"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.managedappregistration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1008

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppRegistration",
      "id": "1a9578ba-78ba-1a95-ba78-951aba78951a",
      "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
      "lastSyncDateTime": "2016-12-31T23:57:45.5058522+00:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "managedDeviceId": "Managed Device Id value",
      "azureADDeviceId": "Azure ADDevice Id value",
      "deviceModel": "Device Model value",
      "deviceManufacturer": "Device Manufacturer value",
      "flaggedReasons": [
        "String"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "version": "Version value"
    }
  ]
}
```

