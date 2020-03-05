---
title: "List deviceConfigurationDeviceOverviews"
description: "List properties and relationships of the deviceConfigurationDeviceOverview objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceConfigurationDeviceOverviews

Namespace: microsoft.graph

List properties and relationships of the [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) objects.

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
GET ** Collection URI for microsoft.graph.deviceConfigurationDeviceOverview not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceOverview](../resources/deviceconfigurationdeviceoverview.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deviceconfigurationdeviceoverview"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.deviceConfigurationDeviceOverview not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceconfigurationdeviceoverview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 402

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
      "id": "a6ed6042-6042-a6ed-4260-eda64260eda6",
      "pendingCount": 12,
      "notApplicableCount": 2,
      "successCount": 12,
      "errorCount": 10,
      "failedCount": 11,
      "lastUpdateDateTime": "2017-01-01T00:03:07.1140227+03:00",
      "configurationVersion": 4
    }
  ]
}
```

