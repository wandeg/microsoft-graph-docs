---
title: "Get device"
description: "Read the properties and relationships of a device object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get device

Namespace: microsoft.graph

Read the properties and relationships of a [device](../resources/device.md) object.

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
GET /devices/{devicesId}
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
If successful, this method returns a `200 OK` response code and a [device](../resources/device.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_device"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{devicesId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.device",
    "id": "6cb60648-0648-6cb6-4806-b66c4806b66c",
    "deletedDateTime": "2016-12-31T23:58:36.4652914+03:00",
    "accountEnabled": true,
    "alternativeSecurityIds": [
      {
        "@odata.type": "microsoft.graph.alternativeSecurityId",
        "type": 4,
        "identityProvider": "Identity Provider value",
        "key": "a2V5"
      }
    ],
    "approximateLastSignInDateTime": "2017-01-01T00:00:06.4864933+03:00",
    "complianceExpirationDateTime": "2017-01-01T00:00:14.119916+03:00",
    "deviceId": "Device Id value",
    "deviceMetadata": "Device Metadata value",
    "deviceVersion": 13,
    "displayName": "Display Name value",
    "isCompliant": true,
    "isManaged": true,
    "mdmAppId": "Mdm App Id value",
    "onPremisesLastSyncDateTime": "2017-01-01T00:03:23.0515041+03:00",
    "onPremisesSyncEnabled": true,
    "operatingSystem": "Operating System value",
    "operatingSystemVersion": "Operating System Version value",
    "physicalIds": [
      "Physical Ids value"
    ],
    "profileType": "Profile Type value",
    "systemLabels": [
      "System Labels value"
    ],
    "trustType": "Trust Type value"
  }
}
```

