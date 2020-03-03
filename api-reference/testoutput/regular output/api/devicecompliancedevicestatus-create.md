---
title: "Create deviceComplianceDeviceStatus"
description: "Create a new deviceComplianceDeviceStatus object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create deviceComplianceDeviceStatus

Namespace: microsoft.graph

Create a new [deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) object.

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
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) object.

The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deviceDisplayName|String|Device name of the DevicePolicyStatus.|
|userName|String|The User Name that is being reported|
|deviceModel|String|The device model that is being reported|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires|
|status|Enumeration|Compliance status of the policy report. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Last modified date time of the policy report.|
|userPrincipalName|String|UserPrincipalName.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/devicecompliancedevicestatus.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicecompliancedevicestatus_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
Content-type: application/json
Content-length: 420

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:58:14.8586698+03:00",
  "status": "String",
  "lastReportedDateTime": "2017-01-01T00:01:14.9975606+03:00",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicecompliancedevicestatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 469

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "e4faae78-ae78-e4fa-78ae-fae478aefae4",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:58:14.8586698+03:00",
  "status": "String",
  "lastReportedDateTime": "2017-01-01T00:01:14.9975606+03:00",
  "userPrincipalName": "User Principal Name value"
}
```

