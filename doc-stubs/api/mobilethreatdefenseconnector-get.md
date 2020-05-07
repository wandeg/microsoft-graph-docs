---
title: "Get mobileThreatDefenseConnector"
description: "Read the properties and relationships of a mobileThreatDefenseConnector object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get mobileThreatDefenseConnector

Namespace: microsoft.graph

Read the properties and relationships of a [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object.

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
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_mobilethreatdefenseconnector"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileThreatDefenseConnector"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

