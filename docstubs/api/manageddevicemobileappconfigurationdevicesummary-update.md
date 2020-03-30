---
title: "Update managedDeviceMobileAppConfigurationDeviceSummary"
description: "Update the properties of a managedDeviceMobileAppConfigurationDeviceSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update managedDeviceMobileAppConfigurationDeviceSummary

Namespace: microsoft.graph

Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md) object.

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
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md) object.

The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|pendingCount|Int32||
|notApplicableCount|Int32||
|notApplicablePlatformCount|Int32||
|successCount|Int32||
|errorCount|Int32||
|failedCount|Int32||
|conflictCount|Int32||
|lastUpdateDateTime|DateTimeOffset||
|configurationVersion|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_manageddevicemobileappconfigurationdevicesummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2017-01-01T00:02:55.5721787+03:00",
  "configurationVersion": 4
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
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "7d6b0384-0384-7d6b-8403-6b7d84036b7d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2017-01-01T00:02:55.5721787+03:00",
  "configurationVersion": 4
}
```

