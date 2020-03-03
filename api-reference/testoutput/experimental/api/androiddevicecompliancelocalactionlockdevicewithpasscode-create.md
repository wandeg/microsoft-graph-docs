---
title: "Create androidDeviceComplianceLocalActionLockDeviceWithPasscode"
description: "Create a new androidDeviceComplianceLocalActionLockDeviceWithPasscode object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create androidDeviceComplianceLocalActionLockDeviceWithPasscode

Create a new [androidDeviceComplianceLocalActionLockDeviceWithPasscode](../resources/androiddevicecompliancelocalactionlockdevicewithpasscode.md) object.

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
POST ** Collection URI for microsoft.graph.androidDeviceComplianceLocalActionLockDeviceWithPasscode not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the androidDeviceComplianceLocalActionLockDeviceWithPasscode object.

The following table shows the properties that are required when you create the androidDeviceComplianceLocalActionLockDeviceWithPasscode.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|gracePeriodInMinutes|Int32|Number of minutes to wait till a local action is enforced. Valid values 0 to 2147483647 Inherited from [androidDeviceComplianceLocalActionBase](../resources/androidDeviceComplianceLocalActionBase.md)|
|passcode|String|Passcode to reset to Android device. This property is read-only.|
|passcodeSignInFailureCountBeforeWipe|Int32|Number of sign in failures before wiping device, the value can be 4-11. Valid values 4 to 11|



## Response
If successful, this method returns a `201 Created` response code and a [androidDeviceComplianceLocalActionLockDeviceWithPasscode](../resources/androiddevicecompliancelocalactionlockdevicewithpasscode.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_androiddevicecompliancelocalactionlockdevicewithpasscode_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.androidDeviceComplianceLocalActionLockDeviceWithPasscode not found
Content-type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.androidDeviceComplianceLocalActionLockDeviceWithPasscode",
  "gracePeriodInMinutes": 4,
  "passcode": "Passcode value",
  "passcodeSignInFailureCountBeforeWipe": 4
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androiddevicecompliancelocalactionlockdevicewithpasscode"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 256

{
  "@odata.type": "#microsoft.graph.androidDeviceComplianceLocalActionLockDeviceWithPasscode",
  "id": "0ae00c04-0c04-0ae0-040c-e00a040ce00a",
  "gracePeriodInMinutes": 4,
  "passcode": "Passcode value",
  "passcodeSignInFailureCountBeforeWipe": 4
}
```

