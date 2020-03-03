---
title: "Add iosUpdateStatuses"
description: "Add iosUpdateStatuses by posting to the iosUpdateStatuses collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add iosUpdateStatuses

Namespace: microsoft.graph

Add iosUpdateStatuses by posting to the iosUpdateStatuses collection.

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
POST /deviceManagement/iosUpdateStatuses/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) object.

The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|installStatus|Enumeration|The installation status of the policy report. Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.|
|osVersion|String|The device version that is being reported.|
|deviceId|String|The device id that is being reported.|
|userId|String|The User id that is being reported.|
|deviceDisplayName|String|Device name of the DevicePolicyStatus.|
|userName|String|The User Name that is being reported|
|deviceModel|String|The device model that is being reported|
|platform|Int32|Platform of the device that is being reported|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires|
|status|Enumeration|Compliance status of the policy report. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Last modified date time of the policy report.|
|userPrincipalName|String|UserPrincipalName.|



## Response
If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_iosupdatedevicestatus_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "String",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2017-01-01T00:02:25.414643+03:00",
  "status": "String",
  "lastReportedDateTime": "2017-01-01T00:01:11.3421719+03:00",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.iosupdatedevicestatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 609

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "5c4ba2ec-a2ec-5c4b-eca2-4b5ceca24b5c",
  "installStatus": "String",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2017-01-01T00:02:25.414643+03:00",
  "status": "String",
  "lastReportedDateTime": "2017-01-01T00:01:11.3421719+03:00",
  "userPrincipalName": "User Principal Name value"
}
```

