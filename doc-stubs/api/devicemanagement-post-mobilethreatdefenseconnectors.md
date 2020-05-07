---
title: "Create mobileThreatDefenseConnectors"
description: "Create a new mobileThreatDefenseConnectors object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create mobileThreatDefenseConnectors

Namespace: microsoft.graph

Create a new mobileThreatDefenseConnectors object.

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
POST /deviceManagement/mobileThreatDefenseConnectors
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.

The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastHeartbeatDateTime|DateTimeOffset|**TODO: Add Description**|
|partnerState|mobileThreatPartnerTenantState|**TODO: Add Description**. Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.|
|androidMobileApplicationManagementEnabled|Boolean|**TODO: Add Description**|
|iosMobileApplicationManagementEnabled|Boolean|**TODO: Add Description**|
|androidEnabled|Boolean|**TODO: Add Description**|
|iosEnabled|Boolean|**TODO: Add Description**|
|windowsEnabled|Boolean|**TODO: Add Description**|
|macEnabled|Boolean|**TODO: Add Description**|
|androidDeviceBlockedOnMissingPartnerData|Boolean|**TODO: Add Description**|
|iosDeviceBlockedOnMissingPartnerData|Boolean|**TODO: Add Description**|
|windowsDeviceBlockedOnMissingPartnerData|Boolean|**TODO: Add Description**|
|macDeviceBlockedOnMissingPartnerData|Boolean|**TODO: Add Description**|
|partnerUnsupportedOsVersionBlocked|Boolean|**TODO: Add Description**|
|partnerUnresponsivenessThresholdInDays|Int32|**TODO: Add Description**|
|allowPartnerToCollectIOSApplicationMetadata|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_mobilethreatdefenseconnector_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
Content-Type: application/json
Content-length: 776

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "androidMobileApplicationManagementEnabled": "Boolean",
  "iosMobileApplicationManagementEnabled": "Boolean",
  "androidEnabled": "Boolean",
  "iosEnabled": "Boolean",
  "windowsEnabled": "Boolean",
  "macEnabled": "Boolean",
  "androidDeviceBlockedOnMissingPartnerData": "Boolean",
  "iosDeviceBlockedOnMissingPartnerData": "Boolean",
  "windowsDeviceBlockedOnMissingPartnerData": "Boolean",
  "macDeviceBlockedOnMissingPartnerData": "Boolean",
  "partnerUnsupportedOsVersionBlocked": "Boolean",
  "partnerUnresponsivenessThresholdInDays": "Integer",
  "allowPartnerToCollectIOSApplicationMetadata": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobilethreatdefenseconnector"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "d68099c8-99c8-d680-c899-80d6c89980d6",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "androidMobileApplicationManagementEnabled": "Boolean",
  "iosMobileApplicationManagementEnabled": "Boolean",
  "androidEnabled": "Boolean",
  "iosEnabled": "Boolean",
  "windowsEnabled": "Boolean",
  "macEnabled": "Boolean",
  "androidDeviceBlockedOnMissingPartnerData": "Boolean",
  "iosDeviceBlockedOnMissingPartnerData": "Boolean",
  "windowsDeviceBlockedOnMissingPartnerData": "Boolean",
  "macDeviceBlockedOnMissingPartnerData": "Boolean",
  "partnerUnsupportedOsVersionBlocked": "Boolean",
  "partnerUnresponsivenessThresholdInDays": "Integer",
  "allowPartnerToCollectIOSApplicationMetadata": "Boolean"
}
```

