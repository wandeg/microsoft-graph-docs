---
title: "Create windowsInformationProtectionDeviceRegistrations"
description: "Create windowsInformationProtectionDeviceRegistrations by posting to the windowsInformationProtectionDeviceRegistrations collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create windowsInformationProtectionDeviceRegistrations

Namespace: microsoft.graph

Create windowsInformationProtectionDeviceRegistrations by posting to the windowsInformationProtectionDeviceRegistrations collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/windowsInformationProtectionDeviceRegistrations/$ref
POST /users/{usersId}/windowsInformationProtectionDeviceRegistrations/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) object.

The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userId|String|UserId associated with this device registration record.|
|deviceRegistrationId|String|Device identifier for this device registration record.|
|deviceName|String|Device name.|
|deviceType|String|Device type, for example, Windows laptop VS Windows phone.|
|deviceMacAddress|String|Device Mac address.|
|lastCheckInDateTime|DateTimeOffset|Last checkin time of the device.|



## Response
If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_windowsinformationprotectiondeviceregistration_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/windowsInformationProtectionDeviceRegistrations
Content-Type: application/json
Content-length: 367

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:57:30.4046407+03:00"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsinformationprotectiondeviceregistration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "bf132102-2102-bf13-0221-13bf022113bf",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:57:30.4046407+03:00"
}
```

