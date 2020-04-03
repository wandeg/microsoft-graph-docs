---
title: "Update mobileThreatDefenseConnector"
description: "Update the properties of a mobileThreatDefenseConnector object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update mobileThreatDefenseConnector

Namespace: microsoft.graph

Update the properties of a [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.

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
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.

The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastHeartbeatDateTime|DateTimeOffset||
|partnerState|Enumeration| Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.|
|androidMobileApplicationManagementEnabled|Boolean||
|iosMobileApplicationManagementEnabled|Boolean||
|androidEnabled|Boolean||
|iosEnabled|Boolean||
|windowsEnabled|Boolean||
|macEnabled|Boolean||
|androidDeviceBlockedOnMissingPartnerData|Boolean||
|iosDeviceBlockedOnMissingPartnerData|Boolean||
|windowsDeviceBlockedOnMissingPartnerData|Boolean||
|macDeviceBlockedOnMissingPartnerData|Boolean||
|partnerUnsupportedOsVersionBlocked|Boolean||
|partnerUnresponsivenessThresholdInDays|Int32||
|allowPartnerToCollectIOSApplicationMetadata|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_mobilethreatdefenseconnector"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 722

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:00.975564+00:00",
  "partnerState": "String",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
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
Content-Length: 771

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "3f51997b-997b-3f51-7b99-513f7b99513f",
  "lastHeartbeatDateTime": "2016-12-31T23:59:00.975564+00:00",
  "partnerState": "String",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```

