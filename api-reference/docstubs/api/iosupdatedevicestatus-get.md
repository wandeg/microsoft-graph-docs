---
title: "Get iosUpdateDeviceStatus"
description: "Read the properties and relationships of an iosUpdateDeviceStatus object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get iosUpdateDeviceStatus

Namespace: microsoft.graph

Read the properties and relationships of an [iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) object.

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
GET /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
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
If successful, this method returns a `200 OK` response code and an [iosUpdateDeviceStatus](../resources/iosupdatedevicestatus.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_iosupdatedevicestatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.iosUpdateDeviceStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
    "id": "9b02f34a-f34a-9b02-4af3-029b4af3029b",
    "installStatus": "String",
    "osVersion": "Os Version value",
    "deviceId": "Device Id value",
    "userId": "User Id value",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:57:34.8473832+03:00",
    "status": "String",
    "lastReportedDateTime": "2017-01-01T00:03:26.8280515+03:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```

