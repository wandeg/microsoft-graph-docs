---
title: "List managedDeviceOverview"
description: "Get the managedDeviceOverviews from the managedDeviceOverview navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List managedDeviceOverview

Namespace: microsoft.graph

Get the managedDeviceOverviews from the managedDeviceOverview navigation property.

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
GET /deviceManagement/managedDeviceOverview
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [managedDeviceOverview](../resources/manageddeviceoverview.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_manageddeviceoverview"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.manageddeviceoverview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceOverview",
      "id": "9cc4dac7-dac7-9cc4-c7da-c49cc7dac49c",
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
        "unknownCount": 12
      },
      "deviceExchangeAccessStateSummary": {
        "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
        "allowedDeviceCount": 2,
        "blockedDeviceCount": 2,
        "quarantinedDeviceCount": 6,
        "unknownDeviceCount": 2,
        "unavailableDeviceCount": 6
      }
    }
  ]
}
```

