---
title: "Create teamsDeviceUsageUserDetail"
description: "Create a new teamsDeviceUsageUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create teamsDeviceUsageUserDetail

Create a new [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) object.

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
POST ** Collection URI for microsoft.graph.teamsDeviceUsageUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the teamsDeviceUsageUserDetail object.

The following table shows the properties that are required when you create the teamsDeviceUsageUserDetail.

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
If successful, this method returns a `201 Created` response code and a [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_teamsdeviceusageuserdetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.teamsDeviceUsageUserDetail not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsdeviceusageuserdetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 465

{
  "@odata.type": "#microsoft.graph.teamsDeviceUsageUserDetail",
  "id": "7b410dca-0dca-7b41-ca0d-417bca0d417b",
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

