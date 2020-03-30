---
title: "Add deviceStatuses"
description: "Add deviceStatuses by posting to the deviceStatuses collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceStatuses

Namespace: microsoft.graph

Add deviceStatuses by posting to the deviceStatuses collection.

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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_deviceconfigurationdevicestatus_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 441

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:57:41.6559639+03:00",
  "status": "String",
  "lastReportedDateTime": "2016-12-31T23:59:04.0371883+03:00",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceconfigurationdevicestatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 490

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "0b2ab9b6-b9b6-0b2a-b6b9-2a0bb6b92a0b",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:57:41.6559639+03:00",
  "status": "String",
  "lastReportedDateTime": "2016-12-31T23:59:04.0371883+03:00",
  "userPrincipalName": "User Principal Name value"
}
```

