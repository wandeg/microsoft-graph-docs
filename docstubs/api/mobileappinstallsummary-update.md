---
title: "Update mobileAppInstallSummary"
description: "Update the properties of a mobileAppInstallSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update mobileAppInstallSummary

Namespace: microsoft.graph

Update the properties of a [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.

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
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.

The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32||
|failedDeviceCount|Int32||
|notApplicableDeviceCount|Int32||
|notInstalledDeviceCount|Int32||
|pendingInstallDeviceCount|Int32||
|installedUserCount|Int32||
|failedUserCount|Int32||
|notApplicableUserCount|Int32||
|notInstalledUserCount|Int32||
|pendingInstallUserCount|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_mobileappinstallsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
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
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "1dd2c84c-c84c-1dd2-4cc8-d21d4cc8d21d",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```

