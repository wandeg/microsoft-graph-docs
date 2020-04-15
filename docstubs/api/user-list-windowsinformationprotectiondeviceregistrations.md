---
title: "List windowsInformationProtectionDeviceRegistrations"
description: "Get the windowsInformationProtectionDeviceRegistrations from the windowsInformationProtectionDeviceRegistrations navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List windowsInformationProtectionDeviceRegistrations

Namespace: microsoft.graph

Get the windowsInformationProtectionDeviceRegistrations from the windowsInformationProtectionDeviceRegistrations navigation property.

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
GET /me/windowsInformationProtectionDeviceRegistrations
GET /users/{usersId}/windowsInformationProtectionDeviceRegistrations
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionDeviceRegistration](../resources/windowsinformationprotectiondeviceregistration.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_windowsinformationprotectiondeviceregistration"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/windowsInformationProtectionDeviceRegistrations
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsinformationprotectiondeviceregistration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

