---
title: "List managedDeviceEncryptionStates"
description: "List properties and relationships of the managedDeviceEncryptionState objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List managedDeviceEncryptionStates

Namespace: microsoft.graph

List properties and relationships of the [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) objects.

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
GET /deviceManagement/managedDeviceEncryptionStates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_manageddeviceencryptionstate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/managedDeviceEncryptionStates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.manageddeviceencryptionstate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 829

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
      "id": "632426d4-26d4-6324-d426-2463d4262463",
      "userPrincipalName": "User Principal Name value",
      "deviceType": "String",
      "osVersion": "Os Version value",
      "tpmSpecificationVersion": "Tpm Specification Version value",
      "deviceName": "Device Name value",
      "encryptionReadinessState": "String",
      "encryptionState": "String",
      "encryptionPolicySettingState": "String",
      "advancedBitLockerStates": "String",
      "fileVaultStates": "String",
      "policyDetails": [
        {
          "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
          "policyId": "Policy Id value",
          "policyName": "Policy Name value"
        }
      ]
    }
  ]
}
```

