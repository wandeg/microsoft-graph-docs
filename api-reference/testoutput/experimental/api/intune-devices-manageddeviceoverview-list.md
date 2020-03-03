---
title: "List managedDeviceOverviews"
description: "List properties and relationships of the managedDeviceOverview objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List managedDeviceOverviews

List properties and relationships of the [managedDeviceOverview](../resources/manageddeviceoverview.md) objects.

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
GET ** Collection URI for microsoft.graph.managedDeviceOverview not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [managedDeviceOverview](../resources/manageddeviceoverview.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_manageddeviceoverview"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.managedDeviceOverview not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.manageddeviceoverview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1372

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceOverview",
      "id": "3b4c1902-1902-3b4c-0219-4c3b02194c3b",
      "enrolledDeviceCount": 3,
      "mdmEnrolledCount": 0,
      "dualEnrolledDeviceCount": 7,
      "deviceOperatingSystemSummary": {
        "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
        "androidCount": 12,
        "iosCount": 8,
        "macOSCount": 10,
        "windowsMobileCount": 2,
        "windowsCount": 12,
        "unknownCount": 12,
        "androidDedicatedCount": 5,
        "androidDeviceAdminCount": 7,
        "androidFullyManagedCount": 8,
        "androidWorkProfileCount": 7
      },
      "deviceExchangeAccessStateSummary": {
        "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
        "allowedDeviceCount": 2,
        "blockedDeviceCount": 2,
        "quarantinedDeviceCount": 6,
        "unknownDeviceCount": 2,
        "unavailableDeviceCount": 6
      },
      "managedDeviceModelsAndManufacturers": {
        "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
        "deviceModels": [
          "Device Models value"
        ],
        "deviceManufacturers": [
          "Device Manufacturers value"
        ]
      },
      "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00"
    }
  ]
}
```

