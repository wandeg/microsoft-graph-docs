---
title: "List teamsDeviceUsageUserCountses"
description: "List properties and relationships of the teamsDeviceUsageUserCounts objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List teamsDeviceUsageUserCountses

Namespace: microsoft.graph

List properties and relationships of the [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) objects.

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
GET ** Collection URI for microsoft.graph.teamsDeviceUsageUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamsdeviceusageusercounts"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.teamsDeviceUsageUserCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsdeviceusageusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 395

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsDeviceUsageUserCounts",
      "id": "fbaefaa7-faa7-fbae-a7fa-aefba7faaefb",
      "reportRefreshDate": "Date",
      "web": 3,
      "windowsPhone": 12,
      "androidPhone": 12,
      "ios": 3,
      "mac": 3,
      "windows": 7,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

