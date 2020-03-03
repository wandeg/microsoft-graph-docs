---
title: "Update yammerDeviceUsageUserDetail"
description: "Update the properties of a yammerDeviceUsageUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update yammerDeviceUsageUserDetail

Update the properties of a [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.yammerDeviceUsageUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [yammerDeviceUsageUserDetail](../resources/yammerDeviceUsageUserDetail.md) object.

The following table shows the properties that are required when you create the [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|userPrincipalName|String||
|displayName|String||
|userState|String||
|stateChangeDate|Date||
|lastActivityDate|Date||
|usedWeb|Boolean||
|usedWindowsPhone|Boolean||
|usedAndroidPhone|Boolean||
|usediPhone|Boolean||
|usediPad|Boolean||
|usedOthers|Boolean||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_yammerdeviceusageuserdetail"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.yammerDeviceUsageUserDetail not found
Content-type: application/json
Content-length: 478

{
  "@odata.type": "#microsoft.graph.yammerDeviceUsageUserDetail",
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
Content-Length: 527

{
  "@odata.type": "#microsoft.graph.yammerDeviceUsageUserDetail",
  "id": "1d1b826e-826e-1d1b-6e82-1b1d6e821b1d",
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
```

