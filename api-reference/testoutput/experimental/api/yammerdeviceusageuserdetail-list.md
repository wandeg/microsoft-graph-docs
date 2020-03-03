---
title: "List yammerDeviceUsageUserDetails"
description: "List properties and relationships of the yammerDeviceUsageUserDetail objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List yammerDeviceUsageUserDetails

Namespace: microsoft.graph

List properties and relationships of the [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) objects.

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
GET ** Collection URI for microsoft.graph.yammerDeviceUsageUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_yammerdeviceusageuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.yammerDeviceUsageUserDetail not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.yammerdeviceusageuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.yammerDeviceUsageUserDetail",
      "id": "301e3a22-3a22-301e-223a-1e30223a1e30",
      "reportRefreshDate": "Date",
      "userPrincipalName": "User Principal Name value",
      "displayName": "Display Name value",
      "userState": "User State value",
      "stateChangeDate": "Date",
      "lastActivityDate": "Date",
      "usedWeb": true,
      "usedWindowsPhone": true,
      "usedAndroidPhone": true,
      "usediPhone": true,
      "usediPad": true,
      "usedOthers": true,
      "reportPeriod": "Report Period value"
    }
  ]
}
```

