---
title: "Update deviceConfigurationState"
description: "Update the properties of a deviceConfigurationState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceConfigurationState

Namespace: microsoft.graph

Update the properties of a [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.

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
PATCH /me/managedDevices/{managedDeviceId}/deviceConfigurationStates/{deviceConfigurationStateId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceConfigurationState](../resources/deviceconfigurationstate.md) object.

The following table shows the properties that are required when you create the [deviceConfigurationState](../resources/deviceconfigurationstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settingStates|[deviceConfigurationSettingState](../resources/deviceconfigurationsettingstate.md) collection||
|displayName|String||
|version|Int32||
|platformType|Enumeration| Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|state|Enumeration| Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|settingCount|Int32||
|userId|String||
|userPrincipalName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationState](../resources/deviceconfigurationstate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_deviceconfigurationstate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/managedDevices/{managedDeviceId}/deviceConfigurationStates/{deviceConfigurationStateId}
Content-type: application/json
Content-length: 1039

{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "String",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1088

{
  "@odata.type": "#microsoft.graph.deviceConfigurationState",
  "id": "183c2145-2145-183c-4521-3c1845213c18",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationSettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "String",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "String",
  "state": "String",
  "settingCount": 12,
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value"
}
```

