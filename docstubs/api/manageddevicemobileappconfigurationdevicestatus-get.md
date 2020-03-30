---
title: "Get managedDeviceMobileAppConfigurationDeviceStatus"
description: "Read properties and relationships of the managedDeviceMobileAppConfigurationDeviceStatus object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get managedDeviceMobileAppConfigurationDeviceStatus

Namespace: microsoft.graph

Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) object.

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
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
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
If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_manageddevicemobileappconfigurationdevicestatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 545

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
    "id": "0e2c18b5-18b5-0e2c-b518-2c0eb5182c0e",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:57:41.6559639+03:00",
    "status": "String",
    "lastReportedDateTime": "2016-12-31T23:59:04.0371883+03:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```

