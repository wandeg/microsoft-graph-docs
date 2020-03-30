---
title: "getTeamsDeviceUsageUserDetail"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getTeamsDeviceUsageUserDetail

Namespace: microsoft.graph



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
GET /reports/getTeamsDeviceUsageUserDetail
GET /print/reports/{reportRootId}/getTeamsDeviceUsageUserDetail
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsdeviceusageuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 554

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsDeviceUsageUserDetail",
      "id": "4a251209-1209-4a25-0912-254a0912254a",
      "reportRefreshDate": "Date",
      "userPrincipalName": "User Principal Name value",
      "lastActivityDate": "Date",
      "isDeleted": true,
      "deletedDate": "Date",
      "usedWeb": true,
      "usedWindowsPhone": true,
      "usediOS": true,
      "usedMac": true,
      "usedAndroidPhone": true,
      "usedWindows": true,
      "reportPeriod": "Report Period value"
    }
  ]
}
```

