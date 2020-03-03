---
title: "Create androidManagedAppRegistration"
description: "Create a new androidManagedAppRegistration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create androidManagedAppRegistration

Namespace: microsoft.graph

Create a new [androidManagedAppRegistration](../resources/androidmanagedappregistration.md) object.

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
POST ** Collection URI for microsoft.graph.androidManagedAppRegistration not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [androidManagedAppRegistration](../resources/androidmanagedappregistration.md) object.

The following table shows the properties that are required when you create the [androidManagedAppRegistration](../resources/androidmanagedappregistration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|Date and time of creation Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|lastSyncDateTime|DateTimeOffset|Date and time of last the app synced with management service. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|applicationVersion|String|App version Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|managementSdkVersion|String|App management SDK version Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|platformVersion|String|Operating System version Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|deviceType|String|Host device type Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|deviceTag|String|App management SDK generated tag, which helps relate apps hosted on the same device. Not guaranteed to relate apps in all conditions. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|deviceName|String|Host device name Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|managedDeviceId|String|The Managed Device identifier of the host device. Value could be empty even when the host device is managed. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|azureADDeviceId|String|The Azure Active Directory Device identifier of the host device. Value could be empty even when the host device is Azure Active Directory registered. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|deviceModel|String|The device model for the current app registration  Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|deviceManufacturer|String|The device manufacturer for the current app registration  Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|flaggedReasons|Enumeration collection|Zero or more reasons an app registration is flagged. E.g. app running on rooted device Inherited from [managedAppRegistration](../resources/managedappregistration.md). Possible values are: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.|
|userId|String|The user Id to who this app registration belongs. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|appIdentifier|[mobileAppIdentifier](../resources/mobileappidentifier.md)|The app package Identifier Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|version|String|Version of the entity. Inherited from [managedAppRegistration](../resources/managedappregistration.md)|
|patchVersion|String|The patch version for the current android app registration|



## Response
If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/androidmanagedappregistration.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_androidmanagedappregistration_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.androidManagedAppRegistration not found
Content-type: application/json
Content-length: 828

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:00:28.8363536+03:00",
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
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidmanagedappregistration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 935

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "id": "4bcbb058-b058-4bcb-58b0-cb4b58b0cb4b",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastSyncDateTime": "2017-01-01T00:00:28.8363536+03:00",
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
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```

