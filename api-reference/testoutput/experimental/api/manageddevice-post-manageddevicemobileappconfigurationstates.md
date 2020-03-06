---
title: "Add managedDeviceMobileAppConfigurationStates"
description: "Add managedDeviceMobileAppConfigurationStates by posting to the managedDeviceMobileAppConfigurationStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add managedDeviceMobileAppConfigurationStates

Namespace: microsoft.graph

Add managedDeviceMobileAppConfigurationStates by posting to the managedDeviceMobileAppConfigurationStates collection.

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
POST /me/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object.

The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|The name of the policy for this policyBase|
|version|Int32|The version of the policy|
|platformType|Enumeration|Platform type that the policy applies to. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|state|Enumeration|The compliance state of the policy. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|settingCount|Int32|Count of how many setting a policy holds|
|userId|String|User unique identifier, must be Guid|
|userPrincipalName|String|User Principal Name|



## Response
If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_manageddevicemobileappconfigurationstate_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates
Content-type: application/json
Content-length: 296

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "String",
  "state": "String",
  "settingCount": 12,
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.manageddevicemobileappconfigurationstate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 345

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "id": "7a2480d3-80d3-7a24-d380-247ad380247a",
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "String",
  "state": "String",
  "settingCount": 12,
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value"
}
```

