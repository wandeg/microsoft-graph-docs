---
title: "List deviceComplianceDeviceOverviews"
description: "List properties and relationships of the deviceComplianceDeviceOverview objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceComplianceDeviceOverviews

Namespace: microsoft.graph

List properties and relationships of the [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) objects.

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
GET ** Collection URI for microsoft.graph.deviceComplianceDeviceOverview not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceOverview](../resources/devicecompliancedeviceoverview.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicecompliancedeviceoverview"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.deviceComplianceDeviceOverview not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicecompliancedeviceoverview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 468

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
      "id": "d226abf5-abf5-d226-f5ab-26d2f5ab26d2",
      "pendingCount": 12,
      "notApplicableCount": 2,
      "notApplicablePlatformCount": 10,
      "successCount": 12,
      "errorCount": 10,
      "failedCount": 11,
      "conflictCount": 13,
      "lastUpdateDateTime": "2017-01-01T00:02:23.4680926+03:00",
      "configurationVersion": 4
    }
  ]
}
```

