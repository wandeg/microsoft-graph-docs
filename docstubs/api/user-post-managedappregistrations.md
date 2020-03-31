---
title: "Create managedAppRegistrations"
description: "Create managedAppRegistrations by posting to the managedAppRegistrations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create managedAppRegistrations

Namespace: microsoft.graph

Create managedAppRegistrations by posting to the managedAppRegistrations collection.

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
POST /me/managedAppRegistrations/$ref
POST /users/{usersId}/managedAppRegistrations/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedAppRegistration](../resources/managedappregistration.md) object.

The following table shows the properties that are required when you create the [managedAppRegistration](../resources/managedappregistration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset||
|lastSyncDateTime|DateTimeOffset||
|applicationVersion|String||
|managementSdkVersion|String||
|platformVersion|String||
|deviceType|String||
|deviceTag|String||
|deviceName|String||
|managedDeviceId|String||
|azureADDeviceId|String||
|deviceModel|String||
|deviceManufacturer|String||
|flaggedReasons|Enumeration collection| Possible values are: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.|
|userId|String||
|appIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)||
|version|String||



## Response
If successful, this method returns a `201 Created` response code and a [managedAppRegistration](../resources/managedappregistration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_managedappregistration_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/managedAppRegistrations
Content-type: application/json
Content-length: 779

{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:03:05.8629729+03:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "String"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedappregistration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 887

{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "id": "9c41dde4-dde4-9c41-e4dd-419ce4dd419c",
  "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
  "lastSyncDateTime": "2017-01-01T00:03:05.8629729+03:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "String"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

