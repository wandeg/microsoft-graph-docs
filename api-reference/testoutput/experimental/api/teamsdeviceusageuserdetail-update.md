---
title: "Update teamsDeviceUsageUserDetail"
description: "Update the properties of a teamsDeviceUsageUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update teamsDeviceUsageUserDetail

Namespace: microsoft.graph

Update the properties of a [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.teamsDeviceUsageUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) object.

The following table shows the properties that are required when you create the [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|userPrincipalName|String||
|lastActivityDate|Date||
|isDeleted|Boolean||
|deletedDate|Date||
|usedWeb|Boolean||
|usedWindowsPhone|Boolean||
|usediOS|Boolean||
|usedMac|Boolean||
|usedAndroidPhone|Boolean||
|usedWindows|Boolean||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_teamsdeviceusageuserdetail"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.teamsDeviceUsageUserDetail not found
Content-type: application/json
Content-length: 416

{
  "@odata.type": "#microsoft.graph.teamsDeviceUsageUserDetail",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 465

{
  "@odata.type": "#microsoft.graph.teamsDeviceUsageUserDetail",
  "id": "fa1e1d91-1d91-fa1e-911d-1efa911d1efa",
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
```

