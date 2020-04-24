---
title: "Get managedDeviceMobileAppConfigurationState"
description: "Read the properties and relationships of a managedDeviceMobileAppConfigurationState object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get managedDeviceMobileAppConfigurationState

Namespace: microsoft.graph

Read the properties and relationships of a [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object.

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
GET /invitations/{invitationsId}/invitedUser/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates/{managedDeviceMobileAppConfigurationStateId}
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
If successful, this method returns a `200 OK` response code and a [managedDeviceMobileAppConfigurationState](../resources/manageddevicemobileappconfigurationstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_manageddevicemobileappconfigurationstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/managedDevices/{managedDeviceId}/managedDeviceMobileAppConfigurationStates/{managedDeviceMobileAppConfigurationStateId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
    "id": "6412df22-df22-6412-22df-126422df1264",
    "settingStates": [
      {
        "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
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
        "currentValue": "Current Value value",
        "settingInstanceId": "Setting Instance Id value"
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
}
```

