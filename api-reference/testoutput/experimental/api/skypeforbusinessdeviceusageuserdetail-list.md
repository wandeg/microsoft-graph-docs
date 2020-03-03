---
title: "List skypeForBusinessDeviceUsageUserDetails"
description: "List properties and relationships of the skypeForBusinessDeviceUsageUserDetail objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List skypeForBusinessDeviceUsageUserDetails

Namespace: microsoft.graph

List properties and relationships of the [skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md) objects.

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
GET ** Collection URI for microsoft.graph.skypeForBusinessDeviceUsageUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_skypeforbusinessdeviceusageuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.skypeForBusinessDeviceUsageUserDetail not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.skypeforbusinessdeviceusageuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 489

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.skypeForBusinessDeviceUsageUserDetail",
      "id": "9bcfcf09-cf09-9bcf-09cf-cf9b09cfcf9b",
      "reportRefreshDate": "Date",
      "userPrincipalName": "User Principal Name value",
      "lastActivityDate": "Date",
      "usedWindows": true,
      "usedWindowsPhone": true,
      "usedAndroidPhone": true,
      "usediPhone": true,
      "usediPad": true,
      "reportPeriod": "Report Period value"
    }
  ]
}
```

