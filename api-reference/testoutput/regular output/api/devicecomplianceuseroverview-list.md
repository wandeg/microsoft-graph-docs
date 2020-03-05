---
title: "List deviceComplianceUserOverviews"
description: "List properties and relationships of the deviceComplianceUserOverview objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceComplianceUserOverviews

Namespace: microsoft.graph

List properties and relationships of the [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) objects.

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
GET ** Collection URI for microsoft.graph.deviceComplianceUserOverview not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserOverview](../resources/devicecomplianceuseroverview.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicecomplianceuseroverview"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.deviceComplianceUserOverview not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicecomplianceuseroverview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
      "id": "934db9b2-b9b2-934d-b2b9-4d93b2b94d93",
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

