---
title: "Create windowsInformationProtectionDeviceRegistration"
description: "Create a new windowsInformationProtectionDeviceRegistration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create windowsInformationProtectionDeviceRegistration

Namespace: microsoft.graph

Create a new [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) object.

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
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) object.

The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userId|String|UserId associated with this device registration record.|
|deviceRegistrationId|String|Device identifier for this device registration record.|
|deviceName|String|Device name.|
|deviceType|String|Device type, for example, Windows laptop VS Windows phone.|
|deviceMacAddress|String|Device Mac address.|
|lastCheckInDateTime|DateTimeOffset|Last checkin time of the device.|



## Response
If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_windowsinformationprotectiondeviceregistration_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/windowsInformationProtectionDeviceRegistrations
Content-type: application/json
Content-length: 367

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:58:23.4652469+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsinformationprotectiondeviceregistration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 416

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "12f95eb0-5eb0-12f9-b05e-f912b05ef912",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:58:23.4652469+03:00"
}
```

