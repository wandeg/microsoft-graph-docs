---
title: "Get windowsInformationProtectionDeviceRegistration"
description: "Read properties and relationships of the windowsInformationProtectionDeviceRegistration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get windowsInformationProtectionDeviceRegistration

Namespace: microsoft.graph

Read properties and relationships of the [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) object.

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
GET /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsinformationprotectiondeviceregistration"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsInformationProtectionDeviceRegistration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
    "id": "cea36699-6699-cea3-9966-a3ce9966a3ce",
    "userId": "User Id value",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceName": "Device Name value",
    "deviceType": "Device Type value",
    "deviceMacAddress": "Device Mac Address value",
    "lastCheckInDateTime": "2017-01-01T00:03:24.7233796+03:00"
  }
}
```

