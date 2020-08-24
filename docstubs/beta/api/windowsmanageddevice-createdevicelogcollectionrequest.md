---
title: "windowsmanageddevice : createDeviceLogCollectionRequest"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# windowsmanageddevice : createDeviceLogCollectionRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

$(this.methodDescription)

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request body

In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this method.

| Parameter    | Type                                                                     | Description |
| :----------- | :----------------------------------------------------------------------- | :---------- |
| templateType | [deviceLogCollectionRequest](../resources/devicelogcollectionrequest.md) |             |

## Response

If successful, this method returns a `200 Ok` response code and a [deviceLogCollectionResponse](../resources/deviceLogCollectionResponse.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "windowsmanageddevice_createdevicelogcollectionrequest"
}
-->

```http
POST https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "errorCode": "Int64",
  "expirationDateTimeUTC": "DateTimeOffset",
  "initiatedByUserPrincipalName": "String",
  "managedDeviceId": "Guid",
  "receivedDateTimeUTC": "DateTimeOffset",
  "requestedDateTimeUTC": "DateTimeOffset",
  "size": "Double",
  "status": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.deviceLogCollectionResponse"
}
-->

```http
HTTP 1.1 200 Ok

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "errorCode": "Int64",
  "expirationDateTimeUTC": "DateTimeOffset",
  "id": "String(identifier)",
  "initiatedByUserPrincipalName": "String",
  "managedDeviceId": "Guid",
  "receivedDateTimeUTC": "DateTimeOffset",
  "requestedDateTimeUTC": "DateTimeOffset",
  "size": "Double",
  "status": "String"
}
}

```