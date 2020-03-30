---
title: "Add mobileThreatDefenseConnectors"
description: "Add mobileThreatDefenseConnectors by posting to the mobileThreatDefenseConnectors collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add mobileThreatDefenseConnectors

Namespace: microsoft.graph

Add mobileThreatDefenseConnectors by posting to the mobileThreatDefenseConnectors collection.

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
POST /deviceManagement/mobileThreatDefenseConnectors/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mobilethreatdefenseconnector_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 723

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2017-01-01T00:00:12.4442527+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.mobilethreatdefenseconnector"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 772

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "5820d07f-d07f-5820-7fd0-20587fd02058",
  "lastHeartbeatDateTime": "2017-01-01T00:00:12.4442527+03:00",
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

