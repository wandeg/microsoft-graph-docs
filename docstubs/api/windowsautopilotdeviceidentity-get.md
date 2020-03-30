---
title: "Get windowsAutopilotDeviceIdentity"
description: "Read properties and relationships of the windowsAutopilotDeviceIdentity object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get windowsAutopilotDeviceIdentity

Namespace: microsoft.graph

Read properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) object.

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
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
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
If successful, this method returns a `200 OK` response code and [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsautopilotdeviceidentity"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsAutopilotDeviceIdentity"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1157

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
    "id": "c2b0b3d2-b3d2-c2b0-d2b3-b0c2d2b3b0c2",
    "deploymentProfileAssignmentStatus": "String",
    "deploymentProfileAssignmentDetailedStatus": "String",
    "deploymentProfileAssignedDateTime": "2016-12-31T23:56:26.7564476+03:00",
    "orderIdentifier": "Order Identifier value",
    "groupTag": "Group Tag value",
    "purchaseOrderIdentifier": "Purchase Order Identifier value",
    "serialNumber": "Serial Number value",
    "productKey": "Product Key value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "enrollmentState": "String",
    "lastContactedDateTime": "2017-01-01T00:03:30.5957753+03:00",
    "addressableUserName": "Addressable User Name value",
    "userPrincipalName": "User Principal Name value",
    "resourceName": "Resource Name value",
    "skuNumber": "Sku Number value",
    "systemFamily": "System Family value",
    "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
    "managedDeviceId": "Managed Device Id value",
    "displayName": "Display Name value"
  }
}
```

