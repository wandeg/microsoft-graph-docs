---
title: "List windowsAutopilotDeviceIdentities"
description: "List properties and relationships of the windowsAutopilotDeviceIdentity objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List windowsAutopilotDeviceIdentities

Namespace: microsoft.graph

List properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) objects.

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
GET /deviceManagement/windowsAutopilotDeviceIdentities
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsautopilotdeviceidentity"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/windowsAutopilotDeviceIdentities
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsautopilotdeviceidentity)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1215

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
      "id": "8e4a7471-7471-8e4a-7174-4a8e71744a8e",
      "deploymentProfileAssignmentStatus": "String",
      "deploymentProfileAssignmentDetailedStatus": "String",
      "deploymentProfileAssignedDateTime": "2017-01-01T00:02:28.5362769+03:00",
      "orderIdentifier": "Order Identifier value",
      "groupTag": "Group Tag value",
      "purchaseOrderIdentifier": "Purchase Order Identifier value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "enrollmentState": "String",
      "lastContactedDateTime": "2016-12-31T23:59:02.6652919+03:00",
      "addressableUserName": "Addressable User Name value",
      "userPrincipalName": "User Principal Name value",
      "resourceName": "Resource Name value",
      "skuNumber": "Sku Number value",
      "systemFamily": "System Family value",
      "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
      "managedDeviceId": "Managed Device Id value",
      "displayName": "Display Name value"
    }
  ]
}
```

