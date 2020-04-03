---
title: "Update deviceConfigurationDeviceStatus"
description: "Update the properties of a deviceConfigurationDeviceStatus object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceConfigurationDeviceStatus

Namespace: microsoft.graph

Update the properties of a [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.

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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.

The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deviceDisplayName|String||
|userName|String||
|deviceModel|String||
|platform|Int32||
|complianceGracePeriodExpirationDateTime|DateTimeOffset||
|status|Enumeration| Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset||
|userPrincipalName|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_deviceconfigurationdevicestatus"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 441

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2017-01-01T00:00:12.5599549+00:00",
  "status": "String",
  "lastReportedDateTime": "2016-12-31T23:57:45.8617849+00:00",
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
Content-Length: 490

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "356e38a0-38a0-356e-a038-6e35a0386e35",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2017-01-01T00:00:12.5599549+00:00",
  "status": "String",
  "lastReportedDateTime": "2016-12-31T23:57:45.8617849+00:00",
  "userPrincipalName": "User Principal Name value"
}
```

